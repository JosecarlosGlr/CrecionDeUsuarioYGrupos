# Creación de usuarios y grupos

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/1.png)

En el apartado **Groups**, he creado el **"Grupo1"** y definido su directorio raíz vinculando la ruta nativa `/home` al punto de montaje virtual `/`. He configurado permisos de **Lectura y Escritura (Read + Write)**, aplicando estas reglas a los subdirectorios.

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/2.png)

Dentro de la pestaña **Limits** del grupo, he establecido límites de velocidad compartidos para todas las sesiones, restringiendo tanto la descarga como la carga a **1000 KiB/s**.

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/3.png)

He creado el **"Usuario1"**, habilitando su cuenta y asignándolo como miembro del **"Grupo1"** para que herede sus permisos y restricciones.

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/4.png)

De igual forma, he creado el **"Usuario2"**, integrándolo en el mismo grupo para mantener una política de acceso uniforme en ambas cuentas.

---

### Diferencias entre Permisos de Usuario y Permisos de Grupo

* **Permisos de Grupo (Plantilla Global):**
  Actúan como una **configuración base**. Se definen una única vez y se aplican automáticamente a todos los usuarios que se añadan a dicho grupo.
  * *Uso principal:* Son ideales para gestionar políticas masivas. Permiten ahorrar tiempo y evitar errores, ya que si necesitas cambiar un permiso para muchos usuarios, solo modificas el grupo una vez.

* **Permisos de Usuario (Configuración Individual):**
  Son configuraciones **específicas** que se aplican a una sola cuenta.
  * *Uso principal:* Se utilizan para gestionar excepciones. Si un usuario concreto necesita acceso a una carpeta extra o un límite de ancho de banda distinto al de sus compañeros, se configura a nivel individual.
  * *Relación:* En FileZilla Server, los permisos de usuario pueden complementar o sobrescribir los heredados del grupo para personalizar la experiencia de acceso.

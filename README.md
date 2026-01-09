# Creción de usuarios y grupos

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/1.png)

Aqui configuro grupo con permisos limitados y defino el directorio raiz

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/2.png)

Defino los limites de conexión de carga y descarga

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/3.png)

Creo el usuario1 y lo agrego al grupo que he creado previamente

![](https://raw.githubusercontent.com/JosecarlosGlr/CrecionDeUsuarioYGrupos/refs/heads/main/4.png)

Creo de igual forma el usuario2 y lo agrego al grupo que he creado previamente

### Diferencias entre Permisos de Usuario y Permisos de Grupo

* **Permisos de Grupo (Plantilla Global):**
  Actúan como una **configuración base**. Se definen una única vez y se aplican automáticamente a todos los usuarios que se añadan a dicho grupo.
  * *Uso principal:* Son ideales para gestionar políticas masivas. Permiten ahorrar tiempo y evitar errores, ya que si necesitas cambiar un permiso para muchos usuarios, solo modificas el grupo una vez.

* **Permisos de Usuario (Configuración Individual):**
  Son configuraciones **específicas** que se aplican a una sola cuenta.
  * *Uso principal:* Se utilizan para gestionar excepciones. Si un usuario concreto necesita acceso a una carpeta extra, mayor ancho de banda o permisos de borrado que el resto de su grupo no tiene, se configuran aquí.
  * *Relación:* Los permisos de usuario suelen tener prioridad o sumarse a los permisos heredados del grupo.

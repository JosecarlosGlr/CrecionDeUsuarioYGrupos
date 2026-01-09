# Creción de usuarios y grupos



# Diferencias entre Permisos de Usuario y Permisos de Grupo

* **Permisos de Grupo (Plantilla Global):**
  Actúan como una **configuración base**. Se definen una única vez y se aplican automáticamente a todos los usuarios que se añadan a dicho grupo.
  * *Uso principal:* Son ideales para gestionar políticas masivas. Permiten ahorrar tiempo y evitar errores, ya que si necesitas cambiar un permiso para muchos usuarios, solo modificas el grupo una vez.

* **Permisos de Usuario (Configuración Individual):**
  Son configuraciones **específicas** que se aplican a una sola cuenta.
  * *Uso principal:* Se utilizan para gestionar excepciones. Si un usuario concreto necesita acceso a una carpeta extra, mayor ancho de banda o permisos de borrado que el resto de su grupo no tiene, se configuran aquí.
  * *Relación:* Los permisos de usuario suelen tener prioridad o sumarse a los permisos heredados del grupo.

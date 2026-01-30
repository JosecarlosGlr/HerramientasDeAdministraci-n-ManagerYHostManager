# Herramientas de administración — Manager y Host Manager

### 1. Web Application Manager (Gestor de Aplicaciones)
Esta herramienta es la interfaz principal para administrar las aplicaciones web (archivos WAR) desplegadas en el servidor.

**Funciones principales investigadas:**
* **Listar Aplicaciones:** Permite ver el estado de todas las apps, su ruta de contexto y el número de sesiones activas.
* **Comandos de Control:** He probado las funciones de Arrancar, Parar, Recargar y Replegar aplicaciones sin necesidad de reiniciar todo el servidor Tomcat.

**Vista general del panel:**
![](https://raw.githubusercontent.com/JosecarlosGlr/HerramientasDeAdministraci-n-ManagerYHostManager/refs/heads/main/1.png)

**Evidencias de la interfaz:**
* **Prueba de parada:** Al pulsar "Parar" en la aplicación `/docs`, el estado cambia a `false` y se deshabilitan las opciones de gestión hasta que se vuelva a arrancar.
![](https://raw.githubusercontent.com/JosecarlosGlr/HerramientasDeAdministraci-n-ManagerYHostManager/refs/heads/main/4.png)


* **Mensaje de confirmación:** Tras realizar una recarga de contexto, la interfaz devuelve un mensaje de éxito en la parte superior.
![](https://raw.githubusercontent.com/JosecarlosGlr/HerramientasDeAdministraci-n-ManagerYHostManager/refs/heads/main/5.png)

* **Despliegue:** Existe una sección específica para cargar archivos `.war` desde el almacenamiento local.
![](https://raw.githubusercontent.com/JosecarlosGlr/HerramientasDeAdministraci-n-ManagerYHostManager/refs/heads/main/6.png)

---

### 2. Virtual Host Manager (Gestor de Máquina Virtual)
Esta interfaz está diseñada para gestionar los "Hosts" o máquinas virtuales dentro del motor de Tomcat, permitiendo que un solo servidor responda a diferentes nombres de dominio.

**Funciones principales investigadas:**
* **Visualización de Hosts:** Permite ver los dominios configurados (por defecto `localhost`).
* **Creación Dinámica:** He investigado el formulario para añadir nuevos hosts especificando su nombre, alias y directorio base de aplicaciones.

**Evidencias de la interfaz:**
* **Configuración de nuevo Host:** He procedido a rellenar el formulario para crear un nuevo host virtual bajo el nombre `www.prueba.com`.
![](https://raw.githubusercontent.com/JosecarlosGlr/HerramientasDeAdministraci-n-ManagerYHostManager/refs/heads/main/7.png)

* **Verificación:** Tras pulsar "Añadir", el nuevo host aparece listado en la tabla de máquinas virtuales activas.
![](https://raw.githubusercontent.com/JosecarlosGlr/HerramientasDeAdministraci-n-ManagerYHostManager/refs/heads/main/8.png)

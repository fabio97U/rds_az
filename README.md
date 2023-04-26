# RDS en Azure

![Diagrama](/arquitectura/Diagrama.drawio.png)

A continuación, se describe brevemente la utilidad de cada uno de los servicios.

- User: usuario de la empresa interno o externo.
- Vpn: conexion a la red capaz de conectarse con el servicio.
- Firewall: capa de seguridad HTTP a nivel de aplicación.
- RDP Web Access: interfaz web para conectarse a la aplicación.
- Server Rds: servidor Windows con los recursos necesarios para todos los usuarios que usaran la aplicación, - tiene configurado el servicio para las conexiones remotas a la aplicación y las licencias de Windows RDLS.
- Disk: discos del servidor con una política de respaldos.
- Logs: espacio donde se almacenará todos los registros de la aplicación, se tendrá el monitoreo de la aplicación y servidor.
- Shared: carpeta de uso compartida entre los usuarios de la aplicación.
- App´s: son las aplicaciones que tendrá disponible los usuarios.
- AD B2C: servicio encargado para la autenticación y autorizacion de los usuarios, tanto internos como - externos a la empresa.
- Terraform Deploy: flujo automatizado para el levantamiento de todos los recursos anteriores. 


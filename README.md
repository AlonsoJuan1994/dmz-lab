#Construcción y Aseguramiento de una Red con una DMZ

 Descripción

Este laboratorio tuvo como objetivo implementar una **Zona Desmilitarizada (DMZ)** utilizando Cisco Packet Tracer. Durante la práctica se configuró una topología de red con tres segmentos (LAN, DMZ y Red Externa), aplicando mecanismos de seguridad como **NAT estático** y **Listas de Control de Acceso (ACL)** para controlar el tráfico entre las diferentes redes.

El objetivo principal fue publicar un servidor web ubicado en la DMZ, permitiendo el acceso desde la red externa sin comprometer la seguridad de la red interna.

 Objetivos

- Configurar el direccionamiento IP de todos los dispositivos.
- Implementar una arquitectura de red con una DMZ.
- Configurar NAT estático para publicar un servidor web.
- Aplicar ACL para controlar y restringir el tráfico entre las distintas redes.
- Validar el funcionamiento mediante pruebas de conectividad y acceso.

Topología de la red

La red está compuesta por tres segmentos:

- **LAN (Red Interna):192.168.1.0/24
- **DMZ (Zona Desmilitarizada): 192.168.2.0/24
- **Red Externa (Internet): 192.168.3.0/24

 Dispositivos utilizados

- Router Cisco ISR 2911 (Router_FW)
- 3 Switches Cisco Catalyst 2960
- PC_Internal
- Server-PT Web_DMZ
- PC_External

 Configuración realizada

Durante el laboratorio se llevaron a cabo las siguientes configuraciones:

- Asignación de direcciones IP a todos los dispositivos.
- Configuración de las interfaces del router.
- Implementación de NAT estático para publicar el servidor web.
- Activación de los servicios HTTP y HTTPS en el servidor de la DMZ.
- Creación y aplicación de ACL para:
  - Permitir únicamente el acceso HTTP desde la red externa.
  - Bloquear el acceso desde la DMZ hacia la red interna.
- Verificación del funcionamiento mediante pruebas de conectividad y acceso web.


 Resultados obtenidos

Se verificó correctamente que:

- Los equipos alcanzan sus respectivos gateways.
- El servidor web es accesible desde la red interna.
- El servidor web es accesible desde la red externa mediante NAT.
- El tráfico ICMP desde Internet hacia la interfaz pública está bloqueado.
- La comunicación iniciada desde la DMZ hacia la LAN está bloqueada.
- El laboratorio fue completado satisfactoriamente con una puntuación de **9/9**.


## Contenido del repositorio

```
.
├── DMZ_PROJECT.pka
├── README.md
├── informe/
│   └── Informe_DMZ_Laboratorio.md
└── evidencias/
    ├── pings-external.png
    ├── pings_server.png
    ├── pc-internal.png
    ├── pexternal-http.png
  

 Tecnologías utilizadas

- Cisco Packet Tracer
- Cisco IOS
- Direccionamiento IPv4
- NAT Estático
- Listas de Control de Acceso (ACL)



Autor

uan Alonso

Bootcamp de Ciberseguridad – 4Geeks Academy

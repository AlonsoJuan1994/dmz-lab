# Construcción y aseguramiento de una red DMZ

**Laboratorio de ciberseguridad | Cisco Packet Tracer | 4Geeks Academy**

## Descripción del proyecto

Diseño e implementación de una red segmentada mediante una zona desmilitarizada (DMZ) utilizando Cisco Packet Tracer. El laboratorio consistió en configurar una infraestructura con tres segmentos de red: LAN interna, DMZ y red externa, aplicando controles de seguridad para proteger los recursos internos.

Se implementaron mecanismos de NAT estático y listas de control de acceso (ACL) para publicar un servidor web en la DMZ, permitiendo el acceso desde la red externa y restringiendo las comunicaciones no autorizadas hacia la LAN.

## Objetivos

- Diseñar y configurar una topología de red segmentada.
- Implementar direccionamiento IPv4 y conectividad entre dispositivos.
- Configurar NAT estático para publicar un servidor web.
- Aplicar ACL para controlar el tráfico entre redes.
- Validar la configuración mediante pruebas de conectividad y acceso HTTP.

## Arquitectura de red

| Segmento | Red |
|---|---|
| LAN interna | 192.168.1.0/24 |
| DMZ | 192.168.2.0/24 |
| Red externa | 192.168.3.0/24 |

**Equipamiento simulado:** router Cisco ISR 2911, tres switches Cisco Catalyst 2960, estaciones de trabajo internas y externas y servidor web ubicado en la DMZ.

## Configuración realizada

Se configuraron las interfaces de red, el direccionamiento IPv4, NAT estático y reglas ACL para permitir el acceso HTTP al servidor publicado y restringir las comunicaciones desde la DMZ hacia la red interna.

También se habilitaron los servicios HTTP y HTTPS del servidor para realizar las pruebas correspondientes.

## Resultados

Las pruebas documentadas permitieron verificar:

- Conectividad de los equipos con sus puertas de enlace.
- Acceso al servidor web desde la LAN interna.
- Acceso HTTP al servidor desde la red externa mediante NAT.
- Bloqueo del tráfico ICMP desde la red externa hacia la interfaz pública.
- Restricción de las conexiones iniciadas desde la DMZ hacia la LAN.

**Resultado del laboratorio: 9/9 puntos**, según la evaluación registrada en el proyecto.

## Herramientas y tecnologías

Cisco Packet Tracer · Cisco IOS · IPv4 · NAT estático · ACL · Segmentación de redes · HTTP/HTTPS

## Archivos y evidencias

- [Abrir laboratorio de Packet Tracer](DMZ_PROJECT.pka)
- [Consultar informe técnico](informe/Informe_DMZ_Laboratorio.md.pdf)
- [Prueba de acceso HTTP externo](evidencias/pexternal-http.png)
- [Prueba de conectividad externa](evidencias/pings-external.png)
- [Prueba de conectividad con el servidor](evidencias/pings_server.png)
- [Evidencia del equipo interno](evidencias/pc-internal%20.png)

## Contexto

Laboratorio académico desarrollado durante la formación en ciberseguridad de 4Geeks Academy, orientado a la implementación de controles de seguridad perimetral y segmentación de redes.

**Autor:** Juan Alonso

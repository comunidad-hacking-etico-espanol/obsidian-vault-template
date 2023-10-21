---
aliases:
  - Servidor Proxy
  - proxy
  - proxies
tags:
  - concepto
---
> [!info] Proxy
> [[Servidor]], programa o dispositivo, que hace de **intermediario en las peticiones de recursos que realiza un cliente a un [[Servidor|servidor]]**.
> 
> ![Diagrama](https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/Open_proxy_h2g2bob.svg/1920px-Open_proxy_h2g2bob.svg.png)
> 
> - Su propósito principal es **filtrar el tráfico peligroso de [[Internet]]**.
> - Permite **ocultar la [[Dirección IP|IP]] del cliente y la ubicación del [[Sitio Web|sitio]]** que visita.
^definicion

> [!EXAMPLE] Caso de uso
> Si una hipotética máquina $A$ solicita un recurso a $C$, lo hará mediante una petición a $B$, que a su vez trasladará la petición a $C$; de esta forma $C$ no sabrá que la petición procedió originalmente de $A$.

Esta situación estratégica de punto intermedio le permite ofrecer diversas funcionalidades:

- Control de acceso
- Registro del tráfico
- Restricción a determinados tipos de tráfico
- Mejora de rendimiento
- [[Anonimato]] de la comunicación
- [[Caché]] web
- (…)

Dependiendo del contexto, la intermediación que realiza el [[Proxy|proxy]] puede ser considerada por los usuarios, administradores o proveedores como legítima o delictiva y **su uso es frecuentemente discutido**.

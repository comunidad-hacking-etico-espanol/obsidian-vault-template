# Introducción

Tanto la [[VPN]] como el [[Proxy|proxy]] se utilizan para **facilitar la conexión entre el cliente y el [[Servidor|servidor]] al ocultar su [[Dirección IP|IP]]** y son ligeramente diferentes en la forma en que manejan los datos.

## ¿Qué es un [[Proxy|proxy]]?

![[Proxy#^definicion]]

### Seguridad de un [[Proxy]]

- Solo **enmascaran la [[Dirección IP|IP]]** del dispositivo y **no cifran los contenidos**.
- Suelen comunicarse con el **protocolo [[HTTP]] o [[SOCKS]]**.

> [!DANGER] Algunas veces los [[Proxy|servidores proxy]] son usados por los ciberdelincuentes
> Estos anuncian un [[Proxy|servidor proxy]] para **robar la identidad de los usuarios**.

Además, los [[Proxy|servidores proxy]] normalmente están *sobrecargados de visitantes* y **afectan terriblemente la velocidad de conexión**.

> [!SUCCESS] Comparado con el [[Proxy|proxy]] normal, *el [[Proxy|proxy]] [[SOCKS5]] es más seguro*
> - Los [[Proxy|proxies]] [[HTTP]] son más familiares y existen desde hace mucho tiempo.
> - Los [[Proxy|proxies]] [[SOCKS5]] se utilizan para conectarse con servicios:
> 	- [[Torrent]].
> 	- [[FTP]].
> 	- [[Servidor|Servidores]] web.
> 
> El [[Proxy|proxy]] [[SOCKS5]] es muy bueno si se usa un [[Torrent]] o un servicio [[P2P]], pero carece de privacidad.
> 
> Si navega mucho por la web y simplemente desea evitar los sitios web bloqueados geográficamente y a través del [[Firewall|firewall]], los [[Proxy|servidores proxy]] son ideales para usted.

## ¿Qué es una [[VPN]]?

![[VPN#^definicion]]

### Seguridad de una [[VPN]]

- Se obtiene una **[[Dirección IP|IP]] única y un túnel seguro** entre el origen y el destino.
- Los servicios de [[VPN]] son **muy fáciles de usar** (encender/apagar el servicio).
- Las aplicaciones [[VPN]] son **compatibles con varias plataformas**.
- **Ocultar la ubicación real** y a acceder a contenido bloqueado o de otros países.

> [!TIP] La clave de las [[VPN|VPNs]] y su punto fuerte, es el **túnel encriptado**
> - Admite el tráfico de todos los protocolos de [[Internet]].
> - Protege los datos incluso conectado a un punto [[WiFi]] abierto.
> - Utiliza protocolos de alta seguridad, como: [[PPTP]], [[L2TP]], [[SSTP]] y [[OpenVPN]].
> - Resulta impenetrable con el uso del cifrado [[AES 256]] y los [[Certificado SSL|certificados SSL]].

# [[Proxy]] VS [[VPN]]

> [!SUCCESS] Cuando se trata de *seguridad* las [[VPN|VPNs]] son **mejores** que los [[Proxy|proxies]]
> Esto se debe a que **las [[VPN|VPNs]] cuentan con un túnel seguro encriptado**.

> [!SUCCESS] Cuando se trata de *velocidad* los [[Proxy|proxies]] son **mejores** que las [[VPN|VPNs]]
> Debido, de nuevo, al **uso de una conexión cifrada por parte de las [[VPN|VPNs]]**, lo que puede **aumentar la latencia y el tiempo de respuesta de la conexión**.
> 
> Además, el cifrado de la conexión [[VPN]] también puede **ralentizar la velocidad de transferencia de datos**.

# Referencias

- Fuente: [Cyber Security News](https://cybersecuritynews.com/vpn-and-proxy/?amp)

PRÁCTICA 7. FUNDAMENTOS DE ETHERNET
========================================
       INFORME DE CONEXIÓN DE RED
========================================

Alumno: Sara Rodríguez Vítores

---------------------------------------------------------------------
 PARTE 1: CONFIGURACIÓN GENERAL (Evidencia del comando "ipconfig /all")
---------------------------------------------------------------------

Configuración IP de Windows

   Nombre de host. . . . . . . . . : CASA
   Sufijo DNS principal  . . . . . :
   Tipo de nodo. . . . . . . . . . : híbrido
   Enrutamiento IP habilitado. . . : no
   Proxy WINS habilitado . . . . . : no
   Lista de búsqueda de sufijos DNS: home

Adaptador desconocido CloudflareWARP:

   Sufijo DNS específico para la conexión. . :
   Descripción . . . . . . . . . . . . . . . : Cloudflare WARP Interface Tunnel
   Dirección física. . . . . . . . . . . . . :
   DHCP habilitado . . . . . . . . . . . . . : no
   Configuración automática habilitada . . . : sí
   Dirección IPv6 . . . . . . . . . . : 2606:4700:110:88c8:a73e:3a0f:fc50:67c2(Preferido)
   Vínculo: dirección IPv6 local. . . : fe80::de5c:4d5c:39d4:8b3f%27(Preferido)
   Dirección IPv4. . . . . . . . . . . . . . : 172.16.0.2(Preferido)
   Máscara de subred . . . . . . . . . . . . : 255.255.255.255
   Puerta de enlace predeterminada . . . . . :
   Servidores DNS. . . . . . . . . . . . . . : 127.0.2.2
                                       127.0.2.3
   NetBIOS sobre TCP/IP. . . . . . . . . . . : habilitado

Adaptador de LAN inalámbrica Wi-Fi 2:

   Estado de los medios. . . . . . . . . . . : medios desconectados
   Sufijo DNS específico para la conexión. . :
   Descripción . . . . . . . . . . . . . . . : Realtek 8852BE-VT Wireless LAN WiFi 6 PCI-E NIC #2
   Dirección física. . . . . . . . . . . . . : BA-82-F2-58-60-0C
   DHCP habilitado . . . . . . . . . . . . . : sí
   Configuración automática habilitada . . . : sí

Adaptador de LAN inalámbrica Wi-Fi 3:

   Estado de los medios. . . . . . . . . . . : medios desconectados
   Sufijo DNS específico para la conexión. . :
   Descripción . . . . . . . . . . . . . . . : Realtek 8852BE-VT Wireless LAN WiFi 6 PCI-E NIC #3
   Dirección física. . . . . . . . . . . . . : BE-82-F2-58-60-0C
   DHCP habilitado . . . . . . . . . . . . . : sí
   Configuración automática habilitada . . . : sí

Adaptador de LAN inalámbrica Wi-Fi:

   Sufijo DNS específico para la conexión. . : home
   Descripción . . . . . . . . . . . . . . . : Realtek 8852BE-VT Wireless LAN WiFi 6 PCI-E NIC
   Dirección física. . . . . . . . . . . . . : B8-82-F2-58-60-0C
   DHCP habilitado . . . . . . . . . . . . . : sí
   Configuración automática habilitada . . . : sí
   Dirección IPv6 . . . . . . . . . . : 2a0c:5a83:7103:b400:79e1:f3b8:161f:a93c(Preferido)
   Dirección IPv6 temporal. . . . . . : 2a0c:5a83:7103:b400:5093:c295:a47c:8954(Preferido)
   Vínculo: dirección IPv6 local. . . : fe80::dbc4:c4e8:c8ff:9a6b%10(Preferido)
   Dirección IPv4. . . . . . . . . . . . . . : 192.168.1.170(Preferido)
   Máscara de subred . . . . . . . . . . . . : 255.255.255.0
   Concesión obtenida. . . . . . . . . . . . : domingo, 7 de diciembre de 2025 11:29:48
   La concesión expira . . . . . . . . . . . : lunes, 8 de diciembre de 2025 11:29:48
   Puerta de enlace predeterminada . . . . . : fe80::fe22:f4ff:fe5a:3770%10
                                       192.168.1.1
   Servidor DHCP . . . . . . . . . . . . . . : 192.168.1.1
   IAID DHCPv6 . . . . . . . . . . . . . . . : 364413682
   DUID de cliente DHCPv6. . . . . . . . . . : 00-01-00-01-30-74-0F-99-B8-82-F2-58-60-0C
   Servidores DNS. . . . . . . . . . . . . . : ::ffff:127.0.2.2
                                       ::ffff:127.0.2.3
                                       127.0.2.2
                                       127.0.2.3
   NetBIOS sobre TCP/IP. . . . . . . . . . . : habilitado



ANÁLISIS DE MI CONFIGURACIÓN:
-----------------------------

1.  **Mi Dirección IPv4:**
    -   *Valor encontrado:* 192.168.1.170
    -   *Explicación:* ¿Qué representa esta dirección? ¿Es un identificador físico o lógico? LA IP privada que identifica a mi portátil en la red local. Es un identificador lógico.
2.  **Mi Dirección Física (MAC):**
    -   *Valor encontrado:* BA-82-F2-58-60-0C (Wifi 2), BE-82-F2-58-60-0C (Wifi 3) y B8-82-F2-58-60-0C (Wifi)
    -   *Explicación:* ¿Qué es esta dirección y quién se la asigna a mi tarjeta de red? Es una dirreción única de cada tarjeta de red, asignada por el fabricante.

3.  **La IP de mi Puerta de Enlace (Router):**
    -   *Valor encontrado:* 192.168.1.1
    -   *Explicación:* ¿Cuál es la función principal de este dispositivo en la red local? ¿Cuándo lo utiliza mi PC? Comunicarse con otras redes externas, por ejemplo para conectarse a internet. Mi PC lo utiliza para comunicarse fuera de la red local. 

4.  **Mi Máscara de Red:**
    -   *Valor encontrado:* 255.255.255.0
    -   *Explicación:* ¿Para qué le sirve a mi ordenador esta "regla"? ¿Qué decisión le ayuda a tomar? Le sirve para saber qué parte de la IP corresponde a la red (255.255.255) y qué parte al host (.0) y así decidir si una IP pertenece a la red local o no. Todos los dispositivos de la red local comparten la parte de red de la máscara (255.255.255)


---------------------------------------------------------------------
 PARTE 2: AGENDA DE RED LOCAL (Evidencia del comando "arp -a")
---------------------------------------------------------------------

Interfaz: 192.168.1.170 --- 0xa
  Dirección de Internet          Dirección física      Tipo
  192.168.1.1           fc-22-f4-5a-37-70     dinámico
  192.168.1.229         68-07-0a-be-29-10     dinámico
  192.168.1.255         ff-ff-ff-ff-ff-ff     estático
  224.0.0.2             01-00-5e-00-00-02     estático
  224.0.0.22            01-00-5e-00-00-16     estático
  224.0.0.251           01-00-5e-00-00-fb     estático
  224.0.0.252           01-00-5e-00-00-fc     estático
  239.255.255.250       01-00-5e-7f-ff-fa     estático
  255.255.255.255       ff-ff-ff-ff-ff-ff     estático

Interfaz: 172.16.0.2 --- 0x1b
  Dirección de Internet          Dirección física      Tipo
  0.0.0.0                                     estático
  2.16.54.158                                 dinámico
  2.16.54.170                                 dinámico
  2.16.54.177                                 dinámico
  2.16.54.183                                 dinámico
  2.16.88.171                                 dinámico
  2.16.88.184                                 dinámico
  2.17.112.163                                dinámico
  2.17.112.225                                dinámico
  2.20.253.68                                 dinámico
  2.20.253.72                                 dinámico
  2.20.253.77                                 dinámico
  2.20.253.80                                 dinámico
  2.20.253.84                                 dinámico
  2.20.253.91                                 dinámico
  2.20.253.94                                 dinámico
  2.20.253.97                                 dinámico
  2.20.253.146                                dinámico
  2.20.253.148                                dinámico
  2.20.253.151                                dinámico
  2.20.253.152                                dinámico
  2.20.253.153                                dinámico
  2.20.253.154                                dinámico
  2.20.253.155                                dinámico
  2.20.253.156                                dinámico
  2.20.253.158                                dinámico
  2.20.253.170                                dinámico
  2.20.253.171                                dinámico
  2.20.253.173                                dinámico
  2.20.253.174                                dinámico
  2.20.253.175                                dinámico
  2.20.253.176                                dinámico
  2.20.253.177                                dinámico
  2.20.253.178                                dinámico
  2.20.253.179                                dinámico
  2.20.253.180                                dinámico
  2.20.253.181                                dinámico
  2.20.253.182                                dinámico
  2.20.253.183                                dinámico
  2.20.253.184                                dinámico
  2.20.253.185                                dinámico
  2.20.253.186                                dinámico
  2.20.253.187                                dinámico
  2.20.253.189                                dinámico
  2.20.253.190                                dinámico
  2.22.209.149                                dinámico
  4.207.247.138                               dinámico
  4.207.247.139                               dinámico
  4.231.128.59                                dinámico
  13.89.178.26                                dinámico
  13.89.178.27                                dinámico
  13.89.179.8                                 dinámico
  13.89.179.10                                dinámico
  13.89.179.14                                dinámico
  13.95.31.18                                 dinámico
  13.107.5.93                                 dinámico
  13.107.136.10                               dinámico
  13.107.138.10                               dinámico
  13.107.139.11                               dinámico
  13.107.213.43                               dinámico
  13.107.246.43                               dinámico
  18.207.85.246                               dinámico
  20.42.65.84                                 dinámico
  20.42.65.85                                 dinámico
  20.42.65.91                                 dinámico
  20.42.73.25                                 dinámico
  20.42.73.27                                 dinámico
  20.42.73.28                                 dinámico
  20.42.73.31                                 dinámico
  20.44.10.122                                dinámico
  20.44.10.123                                dinámico
  20.50.73.10                                 dinámico
  20.50.73.13                                 dinámico
  20.50.80.214                                dinámico
  20.50.88.244                                dinámico
  20.50.201.200                               dinámico
  20.74.67.0                                  dinámico
  20.103.34.206                               dinámico
  20.105.99.58                                dinámico
  20.165.94.63                                dinámico
  20.166.40.66                                dinámico
  20.189.172.32                               dinámico
  20.189.172.33                               dinámico
  20.189.172.73                               dinámico
  20.189.172.76                               dinámico
  20.189.173.1                                dinámico
  20.189.173.2                                dinámico
  20.189.173.3                                dinámico
  20.189.173.5                                dinámico
  20.189.173.7                                dinámico
  20.189.173.9                                dinámico
  20.189.173.10                               dinámico
  20.189.173.13                               dinámico
  20.189.173.14                               dinámico
  20.189.173.17                               dinámico
  20.189.173.27                               dinámico
  20.190.147.1                                dinámico
  20.190.147.2                                dinámico
  20.190.147.3                                dinámico
  20.190.147.5                                dinámico
  20.190.147.6                                dinámico
  20.190.147.7                                dinámico
  20.190.147.9                                dinámico
  20.190.147.10                               dinámico
  20.190.177.19                               dinámico
  20.190.177.20                               dinámico
  20.190.177.21                               dinámico
  20.190.177.25                               dinámico
  20.190.177.83                               dinámico
  20.190.177.84                               dinámico
  20.190.177.85                               dinámico
  20.190.177.88                               dinámico
  20.190.177.146                              dinámico
  20.190.177.147                              dinámico
  20.190.177.148                              dinámico
  20.190.177.149                              dinámico
  20.190.177.152                              dinámico
  20.190.181.0                                dinámico
  20.190.181.2                                dinámico
  20.190.181.3                                dinámico
  20.190.181.4                                dinámico
  20.190.181.5                                dinámico
  20.190.181.6                                dinámico
  20.190.181.23                               dinámico
  20.199.39.224                               dinámico
  20.231.128.66                               dinámico
  20.231.128.67                               dinámico
  20.242.39.171                               dinámico
  23.14.136.8                                 dinámico
  23.14.136.170                               dinámico
  23.14.137.23                                dinámico
  23.14.137.163                               dinámico
  23.14.137.233                               dinámico
  23.14.138.29                                dinámico
  23.22.254.206                               dinámico
  23.46.84.203                                dinámico
  23.220.156.250                              dinámico
  23.223.111.77                               dinámico
  31.13.83.51                                 dinámico
  34.120.62.213                               dinámico
  34.233.49.149                               dinámico
  35.186.225.202                              dinámico
  35.190.80.1                                 dinámico
  35.241.26.164                               dinámico
  40.69.42.241                                dinámico
  40.79.141.152                               dinámico
  40.79.141.153                               dinámico
  40.79.150.122                               dinámico
  40.79.173.40                                dinámico
  40.97.4.1                                   dinámico
  40.97.188.226                               dinámico
  40.97.190.18                                dinámico
  40.99.153.130                               dinámico
  40.99.213.98                                dinámico
  40.99.217.130                               dinámico
  40.99.220.178                               dinámico
  40.99.220.210                               dinámico
  40.104.46.34                                dinámico
  40.104.46.50                                dinámico
  40.104.46.66                                dinámico
  40.126.49.24                                dinámico
  40.126.49.88                                dinámico
  40.126.49.152                               dinámico
  40.126.53.6                                 dinámico
  40.126.53.7                                 dinámico
  40.126.53.8                                 dinámico
  40.126.53.9                                 dinámico
  40.126.53.10                                dinámico
  40.126.53.11                                dinámico
  40.126.53.12                                dinámico
  40.126.53.14                                dinámico
  40.126.53.15                                dinámico
  40.126.53.16                                dinámico
  40.126.53.17                                dinámico
  40.126.53.18                                dinámico
  40.126.53.21                                dinámico
  40.127.240.158                              dinámico
  44.212.187.117                              dinámico
  51.11.192.51                                dinámico
  51.104.136.2                                dinámico
  51.105.71.136                               dinámico
  51.116.253.168                              dinámico
  51.116.253.170                              dinámico
  51.124.78.146                               dinámico
  51.132.193.104                              dinámico
  51.137.3.17                                 dinámico
  51.138.12.100                               dinámico
  52.5.13.197                                 dinámico
  52.6.228.48                                 dinámico
  52.17.247.109                               dinámico
  52.21.178.111                               dinámico
  52.31.167.175                               dinámico
  52.48.202.212                               dinámico
  52.71.250.211                               dinámico
  52.73.45.44                                 dinámico
  52.96.9.2                                   dinámico
  52.96.9.178                                 dinámico
  52.96.15.178                                dinámico
  52.96.32.178                                dinámico
  52.96.35.178                                dinámico
  52.96.58.98                                 dinámico
  52.96.87.194                                dinámico
  52.96.87.242                                dinámico
  52.96.88.2                                  dinámico
  52.96.88.82                                 dinámico
  52.96.88.114                                dinámico
  52.96.90.34                                 dinámico
  52.96.109.194                               dinámico
  52.96.111.34                                dinámico
  52.96.182.114                               dinámico
  52.96.183.34                                dinámico
  52.97.117.2                                 dinámico
  52.97.117.18                                dinámico
  52.97.117.34                                dinámico
  52.97.117.50                                dinámico
  52.97.201.2                                 dinámico
  52.97.201.50                                dinámico
  52.97.213.162                               dinámico
  52.97.233.18                                dinámico
  52.97.233.66                                dinámico
  52.97.233.98                                dinámico
  52.98.159.194                               dinámico
  52.98.159.226                               dinámico
  52.98.159.242                               dinámico
  52.98.227.130                               dinámico
  52.98.227.146                               dinámico
  52.98.227.162                               dinámico
  52.98.227.226                               dinámico
  52.98.227.242                               dinámico
  52.98.229.2                                 dinámico
  52.98.234.226                               dinámico
  52.98.240.242                               dinámico
  52.98.241.2                                 dinámico
  52.98.248.194                               dinámico
  52.98.248.210                               dinámico
  52.98.250.162                               dinámico
  52.98.250.178                               dinámico
  52.102.116.0                                dinámico
  52.102.116.1                                dinámico
  52.102.116.2                                dinámico
  52.102.116.3                                dinámico
  52.102.116.4                                dinámico
  52.102.116.5                                dinámico
  52.102.116.6                                dinámico
  52.102.116.7                                dinámico
  52.109.0.35                                 dinámico
  52.109.28.47                                dinámico
  52.109.28.48                                dinámico
  52.109.68.9                                 dinámico
  52.109.76.240                               dinámico
  52.109.89.18                                dinámico
  52.109.89.19                                dinámico
  52.109.89.119                               dinámico
  52.110.2.129                                dinámico
  52.110.2.130                                dinámico
  52.110.2.131                                dinámico
  52.110.2.132                                dinámico
  52.110.2.133                                dinámico
  52.110.2.134                                dinámico
  52.110.2.135                                dinámico
  52.110.2.136                                dinámico
  52.110.2.137                                dinámico
  52.110.2.138                                dinámico
  52.110.2.139                                dinámico
  52.110.2.140                                dinámico
  52.110.2.141                                dinámico
  52.110.2.142                                dinámico
  52.110.2.143                                dinámico
  52.110.2.144                                dinámico
  52.110.2.145                                dinámico
  52.110.2.146                                dinámico
  52.110.2.147                                dinámico
  52.110.2.148                                dinámico
  52.110.2.149                                dinámico
  52.110.2.153                                dinámico
  52.110.2.154                                dinámico
  52.110.2.155                                dinámico
  52.110.2.156                                dinámico
  52.110.2.157                                dinámico
  52.110.2.158                                dinámico
  52.110.2.159                                dinámico
  52.110.2.160                                dinámico
  52.110.2.161                                dinámico
  52.110.2.162                                dinámico
  52.110.2.163                                dinámico
  52.110.2.164                                dinámico
  52.110.2.165                                dinámico
  52.110.2.166                                dinámico
  52.110.2.167                                dinámico
  52.110.2.168                                dinámico
  52.110.2.169                                dinámico
  52.110.2.170                                dinámico
  52.110.2.171                                dinámico
  52.110.2.172                                dinámico
  52.110.2.173                                dinámico
  52.110.2.174                                dinámico
  52.110.2.175                                dinámico
  52.110.2.176                                dinámico
  52.110.2.177                                dinámico
  52.110.2.178                                dinámico
  52.110.2.181                                dinámico
  52.110.2.182                                dinámico
  52.110.2.183                                dinámico
  52.110.2.184                                dinámico
  52.110.2.185                                dinámico
  52.110.2.186                                dinámico
  52.110.2.187                                dinámico
  52.110.2.188                                dinámico
  52.110.2.189                                dinámico
  52.110.2.190                                dinámico
  52.110.2.193                                dinámico
  52.110.2.194                                dinámico
  52.110.2.195                                dinámico
  52.110.2.196                                dinámico
  52.110.2.197                                dinámico
  52.110.2.198                                dinámico
  52.110.2.199                                dinámico
  52.110.2.200                                dinámico
  52.110.2.202                                dinámico
  52.110.2.203                                dinámico
  52.111.231.13                               dinámico
  52.111.231.66                               dinámico
  52.111.231.68                               dinámico
  52.111.236.63                               dinámico
  52.111.243.30                               dinámico
  52.111.243.72                               dinámico
  52.111.243.73                               dinámico
  52.123.128.14                               dinámico
  52.123.129.14                               dinámico
  52.168.117.168                              dinámico
  52.168.117.170                              dinámico
  52.168.117.175                              dinámico
  52.178.17.234                               dinámico
  52.182.141.63                               dinámico
  52.182.143.208                              dinámico
  52.182.143.209                              dinámico
  52.182.143.210                              dinámico
  52.182.143.213                              dinámico
  52.202.204.11                               dinámico
  54.144.73.197                               dinámico
  63.140.62.120                               dinámico
  63.140.62.139                               dinámico
  63.140.62.172                               dinámico
  63.140.62.200                               dinámico
  63.140.62.210                               dinámico
  63.140.62.236                               dinámico
  64.233.166.188                              dinámico
  64.233.167.188                              dinámico
  64.233.184.188                              dinámico
  66.102.1.188                                dinámico
  72.144.129.207                              dinámico
  72.145.26.121                               dinámico
  72.145.35.106                               dinámico
  72.145.35.118                               dinámico
  72.153.5.112                                dinámico
  72.154.7.96                                 dinámico
  72.154.7.105                                dinámico
  74.125.71.188                               dinámico
  74.125.206.188                              dinámico
  74.178.76.128                               dinámico
  74.178.240.61                               dinámico
  74.179.71.159                               dinámico
  93.123.17.252                               dinámico
  95.100.109.76                               dinámico
  95.100.109.81                               dinámico
  95.100.109.84                               dinámico
  95.100.109.90                               dinámico
  95.100.109.91                               dinámico
  95.100.109.92                               dinámico
  95.100.109.100                              dinámico
  95.100.109.105                              dinámico
  96.16.86.9                                  dinámico
  96.16.86.10                                 dinámico
  96.16.86.21                                 dinámico
  96.16.86.35                                 dinámico
  96.16.86.36                                 dinámico
  96.16.86.39                                 dinámico
  96.16.88.154                                dinámico
  96.16.88.183                                dinámico
  104.16.174.226                              dinámico
  104.16.175.226                              dinámico
  104.18.32.47                                dinámico
  104.18.38.233                               dinámico
  104.18.41.158                               dinámico
  104.208.16.89                               dinámico
  104.208.16.90                               dinámico
  104.208.16.91                               dinámico
  104.208.16.92                               dinámico
  107.22.247.231                              dinámico
  108.157.113.14                              dinámico
  108.157.113.28                              dinámico
  108.157.113.81                              dinámico
  108.157.113.120                             dinámico
  108.157.128.6                               dinámico
  108.157.128.32                              dinámico
  108.157.128.41                              dinámico
  108.177.15.188                              dinámico
  128.85.113.132                              dinámico
  128.85.113.133                              dinámico
  134.33.185.100                              dinámico
  135.233.45.223                              dinámico
  135.233.95.144                              dinámico
  135.236.137.147                             dinámico
  140.82.112.21                               dinámico
  140.82.112.22                               dinámico
  140.82.113.21                               dinámico
  140.82.113.22                               dinámico
  140.82.114.21                               dinámico
  140.82.114.22                               dinámico
  140.82.121.3                                dinámico
  140.82.121.4                                dinámico
  140.82.121.5                                dinámico
  140.82.121.6                                dinámico
  142.250.178.131                             dinámico
  142.250.178.170                             dinámico
  142.250.178.174                             dinámico
  142.250.179.99                              dinámico
  142.250.179.106                             dinámico
  142.250.184.6                               dinámico
  142.250.184.10                              dinámico
  142.250.184.14                              dinámico
  142.250.184.22                              dinámico
  142.250.184.163                             dinámico
  142.250.184.170                             dinámico
  142.250.184.174                             dinámico
  142.250.184.182                             dinámico
  142.250.185.3                               dinámico
  142.250.185.4                               dinámico
  142.250.185.10                              dinámico
  142.250.185.14                              dinámico
  142.250.185.22                              dinámico
  142.250.200.65                              dinámico
  142.250.200.72                              dinámico
  142.250.200.74                              dinámico
  142.250.200.78                              dinámico
  142.250.200.86                              dinámico
  142.250.200.98                              dinámico
  142.250.200.99                              dinámico
  142.250.200.100                             dinámico
  142.250.200.106                             dinámico
  142.250.200.110                             dinámico
  142.250.200.118                             dinámico
  142.250.200.138                             dinámico
  142.250.200.142                             dinámico
  142.250.200.150                             dinámico
  142.250.200.234                             dinámico
  142.251.15.94                               dinámico
  142.251.39.195                              dinámico
  142.251.39.202                              dinámico
  142.251.140.225                             dinámico
  142.251.140.228                             dinámico
  142.251.140.234                             dinámico
  142.251.140.246                             dinámico
  142.251.142.3                               dinámico
  142.251.173.188                             dinámico
  150.171.22.11                               dinámico
  150.171.22.17                               dinámico
  150.171.27.11                               dinámico
  150.171.28.11                               dinámico
  150.171.73.16                               dinámico
  150.171.74.16                               dinámico
  151.101.1.91                                dinámico
  151.101.65.91                               dinámico
  151.101.129.91                              dinámico
  151.101.134.172                             dinámico
  151.101.193.91                              dinámico
  157.88.21.75                                dinámico
  157.88.25.36                                dinámico
  157.240.5.60                                dinámico
  157.240.202.60                              dinámico
  162.125.21.3                                dinámico
  162.125.68.12                               dinámico
  162.125.68.13                               dinámico
  162.125.68.17                               dinámico
  162.125.68.18                               dinámico
  162.125.68.19                               dinámico
  162.159.36.1                                dinámico
  162.159.46.1                                dinámico
  162.159.137.65                              dinámico
  162.159.138.65                              dinámico
  162.159.142.9                               dinámico
  162.159.197.4                               dinámico
  162.247.241.14                              dinámico
  172.64.146.98                               dinámico
  172.64.149.23                               dinámico
  172.64.155.209                              dinámico
  172.184.231.71                              dinámico
  172.217.17.10                               dinámico
  172.217.17.14                               dinámico
  172.217.18.202                              dinámico
  172.217.19.138                              dinámico
  172.217.168.163                             dinámico
  172.217.168.168                             dinámico
  172.217.168.170                             dinámico
  172.217.168.174                             dinámico
  172.217.168.182                             dinámico
  173.194.76.188                              dinámico
  185.199.108.153                             dinámico
  185.199.109.153                             dinámico
  185.199.110.153                             dinámico
  185.199.111.153                             dinámico
  192.147.130.166                             dinámico
  192.178.132.94                              dinámico
  192.178.223.84                              dinámico
  192.228.79.201                              dinámico
  199.232.210.172                             dinámico
  199.232.214.172                             dinámico
  216.58.209.74                               dinámico
  216.58.209.86                               dinámico
  216.58.214.78                               dinámico
  216.58.214.163                              dinámico
  216.58.214.170                              dinámico
  216.58.215.35                               dinámico
  216.58.215.130                              dinámico
  216.58.215.138                              dinámico
  216.58.215.150                              dinámico
  216.58.215.163                              dinámico
  216.58.215.170                              dinámico
  216.58.215.174                              dinámico
  216.58.215.182                              dinámico
  216.239.34.157                              dinámico
  224.0.0.22                                  estático
  224.0.0.251                                 estático
  224.0.0.252                                 estático
  239.255.255.250                             estático
  255.255.255.255                             estático



ANÁLISIS DE MI TABLA ARP:
-------------------------

Busca en la tabla la línea que corresponde a la IP de tu router (la que encontraste en la Parte 1).

1.  **Entrada del Router en la Tabla ARP:**
    -   *Dirección IP del Router:* 192.168.1.170
    -   *Dirección Física (MAC) del Router:* fc-22-f4-5a-37-70

2.  **Análisis de esta entrada:**
    -   *Explicación:* ¿Qué "traducción" o "mapeo" está mostrando esta línea? ¿Por qué es fundamental que tu PC conozca esta información para poder comunicarse fuera de la red local?
    - Es la traducción de la dirección IP privada del router a su dirección física (MAC). Es fundamental porque para que mi PC pueda enviar datos fuera de la red local, necesita saber la dirección MAC del router.
```

### Paso 3: Conocimientos no suministrados en el tema
Desarrolla brevemente aquí los conceptos que has tenido que asimilar por tu cuenta por no estar reflejados en el tema.

```1. Máscara de subred'''
```2. Formato de la dirección MAC'''
```3. API. Es una “puerta” o interfaz que un software ofrece para que otro software pueda usar sus funciones o acceder a sus datos. La API recibe solicitudes, las envía al sistema interno y devuelve respuestas'''
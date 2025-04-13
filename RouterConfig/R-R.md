# Configuración Router - Router

1. Apagar Router
2. Colocar HWIT

Esta es una configuración para dos sub redes y finalmente la conexión al otro Router

|   Comando          |   Descripción     |
| ---------------    | ----------------  |
| enable             |   Privilegios     |
| interface gig0/0   | Interfaz          |
| ip address IP MASK | direccionamiento  |
| no shutdown        | Encendemos        |
| exit               | Ahora conf R-R    |
| interface gig0/0   | Interfaz 2        |
| ip address IP MASK | direccionamiento  |
| exit               |                   |
| <mark>ROUTER</mark>|<mark>ROUTER</mark>|
| interface serial 0/0/0 | slot del rout |
| ip address IP MASK | direccionamos     |
| clock rate 128000  | reloj             |
| no shutdown        | encendemos        |
| end                |                   |
| copy running-config startup-config    | Guardamos         |

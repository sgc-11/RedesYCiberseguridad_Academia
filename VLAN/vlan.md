# VLAN
Lan virtual
* Es una agrupación lógica de dispositivos de red en el mismo dominio de difusión que puede abarcar varios segmentos físicos.

* **Switches** para crear las VLAN
* Lógicamente, las VLAN también son subredes
* El Router permite comunicar varias redes que puedan estar en una misma VLAN

## Pertenencia a una VLAN
1. Configuración estática
2. Configuración dinámica
3. VoIP

## Enlaces a VLAN
1. Enlace de acceso
    * Cualquier dispositivo conectado a X puerto estará en el mismo dominio de transmisión.
    * Conectar mi PC al Switch
2. Enlace Troncal
    * Transportar tráfico para varias VLAN
    * Cisco admite
        * ISL
        * 802.1Q

## Beneficios de usar VLAN
Seguridad, Reducción de costos, Mejor rendimiento, Reducción del tamaño de los dominios de difusión, Eficiencia del personal de TI, admin de aplicaciones más simple.

## Tipos de VLAN
1. Datos
    * Transportar datos
2. Predeterminada
    * Todos los puertos del switch
3. Nativa
    * Asignada a puerto troncal 802.1Q
4. Administración
    * Acceder a las capacidades de admin de un switch
    * VLAN1 es la de admin por default.
5. de Voz


Un switch tiene 24 puertos
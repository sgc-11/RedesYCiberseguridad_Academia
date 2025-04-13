# VLAN config

```
show vlan brief
```

Ejemplo

* ID de red: **192.168.1.0/24**
* Un switch con 24 puertos
* Cada dpto 5 dispositivos

En el **Switch**

* Paso 1: Asignar num, por ejemplo, vlan10
```
vlan [numero de VLAN]
```

* Paso 2: Asignar nombre
```
name [nombre de la vlan]
```

* Paso 3: Asignar puertos del switch a cada VLAN
```
interface fastEthernet [num puerto]

switchport mode access

switchport access vlan [num de la vlan a asignar]
```

Repetir proceso para cada interfaz que se desea agregar a una VLAN distinta a la predeterminada.

## Más de un switch
* Si suponemos que se agrega al edificio otro piso que va a tener su propio switch, entonces

1. Conectamos los switch con un enlace troncal (Cable cruzado)

```
interface [interfaz a configurar] # Ej: Gigabit

switchport mode trunk

switchport trunk allowed vlan [vlan que transportará] # Ej: vlan 10, 20
```

Por seguridad, cambiamos el num de la VLAN nativa

```
interface [interfaz de enlace troncal]

switchport trunk native vlan [num de vlan] # Ej: vlan 1000
```

* <mark> A nivel LOCAL si podemos tener el mismo número de VLAN.


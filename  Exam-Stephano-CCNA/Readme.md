
## Topologie

![[Pasted image 20250519114021.png]]

## Adressage IP et sous réseaux
- **Adressage PC1**
```
#VLAN 10
addresse IP : 192.168.100.10
masque de sous réseaux: 255.255.255.0
Default Gateway: 192.168.100.1
```

- **Adressage PC2**
```
#VLAN 20
addresse IP : 192.168.100.70
masque de sous réseaux: 255.255.255.0
Default gateway: 192.168.100.65
```

- **Adressage PC3
```
#VLAN 30
addresse IP : 192.168.100.100
masque de sous réseaux: 255.255.255.0
Default gateway: 192.168.100.65
```
## Configuration VLANs et ports

### Configuration du switch

```
enable
configure terminal
vlan 10
name VLAN10
exit
vlan 20
name VLAN20
exit
vlan 30
name VLAN30
exit

```

### Attribuez les ports aux bon VLANs

```
interface range fa1/1 fa2/1 fa3/1
switchport mode access
exit

interface fa0/1
switchport access vlan 10
exit
interface fa0/2
switchport access vlan 20
exit
interface fa0/3
switchport access vlan 30
exit

```

### Configuration port trunk

```
interface fa0/1
switchport mode trunk
exit


```

### Routage Inter vlan

- **VLAN 10**
```
interface Fa0/0.10
encapsulation dot1Q 10
ip address 192.168.10.1 255.255.255.0
no shutdown
```

## Topologie de base

![[topologie.png]]



## Création des VLANs, attributions des ports, configuration des trunks

### Configuration des VLANS sur SW1 et SW2:
```
enable
configure terminal

# Création des VLANs
vlan 10
 name ADMIN
vlan 20
 name PROF
vlan 30
 name ETUDIANT
vlan 99
 name MANAGEMENT
exit

```

### Attribution des ports à leurs VLANs

- **Sur SW1**:
```
# Admin PC sur Fa0/1 → VLAN 10 (Admin)
interface fa0/1
 switchport mode access
 switchport access vlan 10
exit

# Prof PC sur Fa0/2 → VLAN 20 (Prof)
interface fa0/2
 switchport mode access
 switchport access vlan 20
exit

# Liaison vers SW2 sur Fa0/3 → Trunk
interface fa0/3
 switchport mode trunk
 switchport trunk native vlan 99
exit

```

- **Sur SW2**:
```
# Etudiant PC1 sur Fa1/1 → VLAN 30 (Étudiant1)
interface fa1/1
 switchport mode access
 switchport access vlan 30
exit

# Etudiant PC2 sur Fa2/1 → VLAN 30 (Étudiant2)
interface fa2/1
 switchport mode access
 switchport access vlan 30
exit

# Trunk vers SW1 sur Fa0/1
interface fa0/1
 switchport trunk encapsulation dot1q
 switchport mode trunk
 switchport trunk native vlan 99
exit

```
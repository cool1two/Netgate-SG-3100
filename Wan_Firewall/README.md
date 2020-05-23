# Netgate-SG-3100 (In Progress)

## Configuration Setting for Netgate SG-3100

## **Firewall > Rules >  WAN**

---

```diff
! Firewall > Rules >  WAN > WAN Deny ALL IPv4
```

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default*
    1. Action = Pass
    2. Interface = IOT
    3. Protocol = TCP/UDP
    4. Destination = IOT Net
    4. Destination Port Range = 53 
    5. Description = Allow DNS IoT

![SG-3100 Interfaces > VLANs > 55](images/Interfaces-Vlan-55.png)

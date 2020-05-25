# Netgate-SG-3100 (In Progress)

## Configuration Setting for Netgate SG-3100

## **Firewall > Rules >  WAN**

---

### <span style="color:Orange">Interfaces > LAN </span>

#### *Items Modified From Default -.*

    1. IPv4 Address = 192.168.1.1

![SG-3100 Interfaces > WAN](images/Lan-Interface-Configuration.png)

---

### <span style="color:Orange">Firewall > Rules > LAN > LAN Deny ALL IPv4 </span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -..*

    1. Interface = LAN
    2. Address Family = IPv4
    3. Protocal = ANY
    4. Discription = LAN Deny ALL IPv4

This rule replaces the default DENY and allows us to log events.

![SG-3100 Firewall > Rules > LAN > LAN Deny ALL IPv4](images/Firewall_LAN_Deny_ALL_IPv4.png)

---

### <span style="color:Orange">Firewall > Rules > LAN > LAN Deny ALL IPv6 </span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Interface = LAN
    2. Address Family = IPv6
    3. Protocal = ANY
    4. Discription = LAN Deny ALL IPv6

This rule replaces the default DENY and allows us to log events.

![SG-3100 Firewall > Rules > LAN > LAN Deny ALL IPv6](images/Firewall_LAN_Deny_ALL_IPv6.png)

---

### <span style="color:Orange">Firewall > Rules > LAN > Default Allow LAN IPv4 </span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Interface = LAN
    2. Address Family = IPv4
    3. Protocal = ANY
    4. Source = LAN Net
    5. Destination = ANY
    6. Discription = Default Allow LAN IPv4

![SG-3100 Firewall > Rules > LAN > Default Allow LAN IPv4](images/Firewall_LAN_Allow_ALL_IPv4.png)

---

### <span style="color:Orange">Firewall > Rules > LAN > Default Allow LAN IPv6 </span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Interface = LAN
    2. Address Family = IPv6
    3. Protocal = ANY
    4. Source = LAN Net
    5. Destination = ANY
    6. Discription = Default Allow LAN IPv6

![SG-3100 Firewall > Rules > LAN > Default Allow LAN IPv6](images/Firewall_LAN_Allow_ALL_IPv6.png)

---

## [Return](../README.md)

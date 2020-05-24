# Netgate-SG-3100 (Complete)

## Configuration Setting for Netgate SG-3100

## **Firewall > Rules >  WAN**

---

### <span style="color:Orange">Interfaces > WAN </span>

![WARN +](https://via.placeholder.com/15/FF6A00/000000?text=+) *For Bench Lab Only.*

#### *Items Modified From Default -.*
    1. Block private networks and loopback addresses = Unchecked

![OK +](https://via.placeholder.com/15/4CFF00/000000?text=+) *For Production.*

#### *Items Modified From Default -..*

    1. Block private networks and loopback addresses = Checked

![SG-3100 Interfaces > WAN](images/Wan-Interface-Configuration.png)

---

### <span style="color:Orange"> Firewall > Rules > WAN > WAN Deny ALL IPv4</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Action = Block
    2. Interface = WAN
    3. Protocol = Any
    4. Source = Any
    5. Destination = Any
    6. Description = WAN Deny ALL IPv4

This rule replaces the default DENY and allows us to log events.

![SG-3100 Firewall > Rules > IOT > ALLow ALL](images/Firewall_WAN_Deny_ALL_IPv4.png)

### <span style="color:Orange">Firewall > Rules > WAN > WAN Deny ALL IPv6</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -....*

    1. Action = Block
    2. Interface = WAN
    3. Protocol = Any
    4. Address Family = IPv6
    5. Source = Any
    6. Destination = Any
    7. Description = WAN Deny ALL IPv6

This rule replaces the default DENY and allows us to log events.

![SG-3100 Firewall > Rules > IOT > ALLow ALL](images/Firewall_WAN_Deny_ALL_IPv6.png)

---

#### *Final WAN Firewall Configuration.*

![SG-3100 Interfaces > Interface Assignments](images/Firewall_WAN_Final.png)

---

## [Return](../README.md)

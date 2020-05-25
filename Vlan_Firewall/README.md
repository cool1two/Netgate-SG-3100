
# Netgate-SG-3100 (Complete)

## Configuration Setting for Netgate SG-3100

## **Firewall / Rules**

---

### <span style="color:Orange"/System / Firewall / Rules / IOT Network / Allow All IoT</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -.*

    1. Action = Pass
    2. Interface = IOT
    3. Protocol = Any
    4. Source = IOT Net
    5. Description = Allow All IoT

![SG-3100 Firewall / Rules / IOT / ALLow ALL](images/Firewall_Rules_Vlan_IOT_Allow_All.png)

---

### <span style="color:Orange"/Firewall / Rules / IOT Network / Block IoT to LAN</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -..*

    1. Action = Block
    2. Interface = IOT
    3. Protocol = Any
    4. Destination = LAN Net
    5. Description = Block IoT / Lan

![SG-3100 Firewall / Rules / IOT / Block IoT to Lan](images/Firewall_Rules_Vlan_IOT_Block_IOT_Lan.png)

---

### <span style="color:Orange"/Firewall / Rules / IOT Network / Block External DNS</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Action = Block
    2. Interface = IOT
    3. Protocol = TCP/UDP
    4. Destination Port Range = 53 
    5. Description = Block DNS IoT

![SG-3100 Firewall / Rules / IOT / Block External DNS](images/Firewall_Rules_Vlan_IOT_Block_Dns.png)

---

### <span style="color:Orange"/Firewall / Rules / IOT Network / Allow PFSense DNS</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -....*

    1. Action = Pass
    2. Interface = IOT
    3. Protocol = TCP/UDP
    4. Destination = IOT Net
    4. Destination Port Range = 53 
    5. Description = Allow DNS IoT

![SG-3100 Firewall / Rules / IOT / Allow PFSense DNS](images/Firewall_Rules_Vlan_IOT_Allow_Dns.png)

---

### <span style="color:Orange"/Firewall / Rules / IOT Network / Final Configuration</span>

![SG-3100 Firewall / Rules / IOT ](images/Firewall_Rules_Vlan_IOT_Final.png)

---

##### All credit for VLANs to 'Lawrence Systems'

[![All Credit for VLANs to 'Lawrence Systems'](https://img.youtube.com/vi/b2w1Ywt081o/0.jpg)](https://www.youtube.com/watch?v=b2w1Ywt081o)

---

## [Return](../README.md)

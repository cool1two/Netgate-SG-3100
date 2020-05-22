# Netgate-SG-3100

## Configuration Setting for Netgate SG-3100

### **Interfaces > VLANs**

#### *Items Modified From Default*

    1. Parent Interface = Lan
    2. VLAN Tag = 55
    3. Description = Internet of Insecure Things.

![SG-3100 Interfaces > VLANs > 55](images/Interfaces-Vlan-55.png)

#### *Repeat for Vlan 65*

    1. Parent Interface = Lan
    2. VLAN Tag = 65
    3. Description = Next Generation Wireless.

![SG-3100 Interfaces > VLANS 65](images/Interfaces-Vlan-65.png)

---

### **Interfaces > Interface Assignments**

#### *Items Modified From Default*

    1. Modify Interface Assignments > Interfaces OPT2 > Network Port = VLAN 55
    2. Modify Interface Assignments > Interfaces OPT3 > Network Port = VLAN 65

![SG-3100 Interfaces > Interface Assignments](images/Interfaces-Interface-Assignments.png)

### **Interfaces > Interface Assignments > OPT2**

#### *Items Modified From Default*

    1. Enable = Checked
    2. Description = Interface of Insecure Things.
    3. IPv4 Address = 192.168.55.1

![SG-3100 Interfaces > Interface Assignments > OPT2](images/Interfaces_OPT2_VLAN.55.png)

### **Interfaces > Interface Assignments > OPT3**

#### *Items Modified From Default*

    1. Enable = Checked
    2. Description = Next Generation Wireless.
    3. IPv4 Address = 192.168.65.1

![SG-3100 Interfaces > Interface Assignments > OPT3](images/Interfaces_OPT2_VLAN.65.png)

#### *Final Interface Assignments Configuration.*

![SG-3100 Interfaces > Interface Assignments](images/Interfaces-Interface-Assignments2.png)

---

## Firewall > Rules

### **Rules > IOT/NGW Network > Allow All**

#### *Items Modified From Default*
    1. Action = Pass
    2. Protocol = Any
    3. Source = IOT Net
    4. Description = Allow All IOT


![SG-3100 Firewall > Rules > IOT > ALLow ALL](images/Firewall_Rules_Vlan_IOT_Allow_All.png)

### **Rules > IOT/NGW Network > Deny**

#### *Items Modified From Default*
    1. Action = Block
    2. Protocol = Any
    3. Destination = LAN Net
    4. Description = Block IOT > Lan


![SG-3100 Firewall > Rules > IOT > ALLow ALL](images/Firewall_Rules_Vlan_IOT_Block_IOT_Lan.png)

---

##### All credit for VLANs to 'Lawrence Systems'

[![All Credit for VLANs to 'Lawrence Systems'](http://img.youtube.com/vi/b2w1Ywt081o/0.jpg)](http://www.youtube.com/watch?v=b2w1Ywt081o)


# [Return](../README.md)

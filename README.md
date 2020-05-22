# Netgate-SG-3100


## Configuration Setting for Netgate SG-3100

--- 

### **System > General Setup**

#### *Items Modified From Default*

    1. Hostname = Gateway
    2. Domain = Workgroup
    3. DNS Server = [ Pihole Address(s) ]
    4. DNS Server Override = Unchecked
    5. Disable DNS Forwarder = Checked

![SG-3100 System > General Setup](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/System-General-Setup.png)

---

### **Interfaces > VLANs**

#### *Items Modified From Default*

    1. Parent Interface = Lan
    2. VLAN Tag = 55
    3. Description = Internet of Insecure Things.

![SG-3100 Interfaces > VLANs > 55](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Vlan-55.png)

#### *Repeat for Vlan 65*

    1. Parent Interface = Lan
    2. VLAN Tag = 65
    3. Description = Next Generation Wireless.

![SG-3100 Interfaces > VLANS 65](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Vlan-65.png)

### **Interfaces > Interface Assignments**

#### *Items Modified From Default*

    1. Modify Interface Assignments > Interfaces OPT2 > Network Port = VLAN 55
    2. Modify Interface Assignments > Interfaces OPT3 > Network Port = VLAN 65

![SG-3100 Interfaces > Interface Assignments](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Interface-Assignments.png)

### **Interfaces > Interface Assignments > OPT2**

#### *Items Modified From Default*

    1. Enable = Checked
    2. Description = Interface of Insecure Things.
    3. IPv4 Address = 192.168.55.1

![SG-3100 Interfaces > Interface Assignments > OPT2](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces_OPT2_VLAN.55.png)

### **Interfaces > Interface Assignments > OPT3**

#### *Items Modified From Default*

    1. Enable = Checked
    2. Description = Next Generation Wireless.
    3. IPv4 Address = 192.168.65.1

![SG-3100 Interfaces > Interface Assignments > OPT3](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces_OPT2_VLAN.65.png)

#### *Final Interface Assignments Configuration.*

![SG-3100 Interfaces > Interface Assignments](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Interface-Assignments2.png)


[![All Credit for VLANs to 'Lawrence Systems'](http://img.youtube.com/vi/b2w1Ywt081o/0.jpg)](http://www.youtube.com/watch?v=YOUTUb2w1Ywt081o)
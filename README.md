# Netgate-SG-3100


## Configuration Setting for Netgate SG-3100

--- 
- [Netgate-SG-3100](#netgate-sg-3100)
  * [Configuration Setting for Netgate SG-3100](#configuration-setting-for-netgate-sg-3100)
    + [**System > General Setup**](#--system---general-setup--)
      - [*Items Modified From Default*](#-items-modified-from-default-)
    + [**Interfaces > VLANs**](#--interfaces---vlans--)
      - [*Items Modified From Default*](#-items-modified-from-default--1)
      - [*Repeat for Vlan 65*](#-repeat-for-vlan-65-)
    + [**Interfaces > Interface Assignments**](#--interfaces---interface-assignments--)
      - [*Items Modified From Default*](#-items-modified-from-default--2)
    + [**Interfaces > Interface Assignments > OPT2**](#--interfaces---interface-assignments---opt2--)
      - [*Items Modified From Default*](#-items-modified-from-default--3)
    + [**Interfaces > Interface Assignments > OPT3**](#--interfaces---interface-assignments---opt3--)
      - [*Items Modified From Default*](#-items-modified-from-default--4)
      - [*Final Interface Assignments Configuration.*](#-final-interface-assignments-configuration-)
        * [All credit for VLANs to 'Lawrence Systems'](#all-credit-for-vlans-to--lawrence-systems-)
    + [Firewall](#firewall)
---

### [System > General Setup](General_Setup/GENERAL.md)

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

---

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

##### All credit for VLANs to 'Lawrence Systems'

[![All Credit for VLANs to 'Lawrence Systems'](http://img.youtube.com/vi/b2w1Ywt081o/0.jpg)](http://www.youtube.com/watch?v=b2w1Ywt081o)

---

### Firewall 
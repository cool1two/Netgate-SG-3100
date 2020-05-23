# Netgate-SG-3100 (Complete)

## Configuration Setting for Netgate SG-3100

## **Interfaces > VLANs**

---

## Interfaces > VLANs > VLAN Interfaces

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin adding VLAN 55.*

### *Items Modified From Default*

    1. Parent Interface = Lan
    2. VLAN Tag = 55
    3. Description = Internet of Insecure Things.

![SG-3100 Interfaces > VLANs > 55](images/Interfaces-Vlan-55.png)


---

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin adding VLAN 65.*

### *Repeat for Vlan 65*

    1. Parent Interface = Lan
    2. VLAN Tag = 65
    3. Description = Next Generation Wireless.

![SG-3100 Interfaces > VLANS 65](images/Interfaces-Vlan-65.png)

---

### **Interfaces > Interface Assignments**

![Click](https://via.placeholder.com/15/FFD800/000000?text=+) `Use the Dropdown to modify`

#### *Items Modified From Default*

    1. Modify Interface Assignments > Interfaces OPT2 > Network Port = VLAN 55
    2. Modify Interface Assignments > Interfaces OPT3 > Network Port = VLAN 65

![SG-3100 Interfaces > Interface Assignments](images/Interfaces-Interface-Assignments.png)

---

### **Interfaces > Interface Assignments > OPT2**

![Click](https://via.placeholder.com/15/FFD800/000000?text=+) `Click on OPT2 to being editing`

#### *Items Modified From Default*

    1. Enable = Checked
    2. Description = Interface of Insecure Things.
    3. IPv4 Address = 192.168.55.1

![SG-3100 Interfaces > Interface Assignments > OPT2](images/Interfaces_OPT2_VLAN.55.png)

---

### **Interfaces > Interface Assignments > OPT3**

![Click](https://via.placeholder.com/15/FFD800/000000?text=+) `Click on OPT3 to being editing`

#### *Items Modified From Default*

    1. Enable = Checked
    2. Description = Next Generation Wireless.
    3. IPv4 Address = 192.168.65.1

![SG-3100 Interfaces > Interface Assignments > OPT3](images/Interfaces_OPT2_VLAN.65.png)

---

#### *Final Interface Assignments Configuration.*

![SG-3100 Interfaces > Interface Assignments](images/Interfaces-Interface-Assignments2.png)

---

##### All credit for VLANs to 'Lawrence Systems'

[![All Credit for VLANs to 'Lawrence Systems'](https://img.youtube.com/vi/b2w1Ywt081o/0.jpg)](https://www.youtube.com/watch?v=b2w1Ywt081o)

---

# [Return](../README.md)
# Netgate-SG-3100

## Configuration Setting for Netgate SG-3100

---

If you want to embed images, this is how you do it:

![Image of Yaktocat](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/yaktocat.png)

---

## System > General Setup

### Items Modified From Default

1. Hostname = Gateway
2. Domain = Workgroup
3. DNS Server = [ Pihole Address(s) ]
4. DNS Server Override = Unchecked
5. Disable DNS Forwarder = Checked

![SG-3100 System > General Setup ](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/System-General-Setup.png)

---

## Interfaces > VLANs

### Items Modified From Default

1. Parent Interface = Lan
2. VLAN Tag = 55
3. Description = Internet of Insecure Things.

![SG-3100 Interfaces > Vlan ](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Vlan-55.png)

#### Repeat for Vlan 65

1. Parent Interface = Lan
2. VLAN Tag = 55
3. Description = Next Generation Wireless.

![SG-3100 Interfaces > Vlan ](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Vlan-65.png)

## Interfaces > Interface Assignments

### Items Modified From Default

1. Modify Interface > Network Port = OPT2 > VLAN 55
1. Modify Interface > Network Port = OPT3 > VLAN 65

![SG-3100 Interfaces > Vlan ](https://github.com/cool1two/Netgate-SG-3100/blob/n00000001/images/Interfaces-Interface-Assignments.png)
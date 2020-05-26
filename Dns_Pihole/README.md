# Netgate-SG-3100 (Complete)

## Configuration Setting for Netgate SG-3100

## **Services / DNS Resolver / General**

---

### <span style="color:Orange">Services / DNS Resolver / General Settings</span>

#### *Items Modified From Default -.*

    1. Network Interfaces = All
    2. Outgoing Network Interfaces = All
    3. System Domain Local Zone Type = Refuse
    4. DNS Query Forwarding = Checked
    5. DHCP Registration = Checked
    6. Static DHCP = Checked

![SG-3100 / Services / DNS Resolver / General Setting](images/Service_Dns_Resolver_General.png)

---

### <span style="color:Orange">Firewall / NAT / Port Forward</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -..*

    1. Interface = LAN
    2. Protocol = TCP/UDP
    3. Source = (Invert = Checked) Single Host or Alias (Pihole_Dns)
        # Sorce is not Pihole DNS
    4. Destination = (Invert = Checked) LAN net
        # Destination is not LAN
    5. Destination port range = DNS (53)
    6. Redirect target = 127.0.0.1
    7. Redirect target port = DNS (53)
    8.. Description =  Redirect DNS
    9. NAT reflection = Disabled

![SG-3100 / Firewall / NAT / Port Forward](images/Firewall_Nat_PortForward.png)

---

### <span style="color:Orange">Firewall / Rules / LAN / Block DNS Catchall</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Action = Block
    2. Interface = LAN
    3. Address Family = IPv4
    4. Protocol = TCP/UDP
    5. Source = Any
    6. Destination = Any
    7. Destination Port Range = DNS (53)
    8. Description = Block DNS Catchall
    9. Log = Checked

![SG-3100 / Firewall / Rules / LAN / Block DNS Catchall](images/Firewall_Rules_Lan_Block_Dns.png)

---

### <span style="color:Orange">Firewall / Rules / LAN / Permit OpenDNS</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...*

    1. Action = Pass
    2. Interface = LAN
    3. Address Family = IPv4
    4. Protocol = TCP/UDP
    5. Source = Single host or alias (Alias = Pihole_Dns)
    6. Destination = Single host or alias (Alias = Open_Dns)
    7. Destination Port Range = DNS (53)
    8. Description = Permit OpenDNS

![SG-3100 / Firewall / Rules / LAN / Permit OpenDNS](images/Firewall_Rules_Lan_Open_Dns.png)

---

### <span style="color:Orange">Firewall / Rules / LAN / Allow Firewall DNS</span>

![ADD +](https://via.placeholder.com/15/43A047/000000?text=+) *Click Add to begin.*

#### *Items Modified From Default -...'*

    1. Action = Pass
    2. Interface = LAN
    3. Address Family = IPv4
    4. Protocol = TCP/UDP
    5. Source = Any
    6. Destination = This Firewall (self)
    7. Destination Port Range = DNS (53)
    8. Description = Allow Firewall DNS

![SG-3100 / Firewall / Rules / LAN / Allow Firewall DNS](images/Firewall_Rules_Lan_Allow_Firewall_Dns.png)

---

#### *Final WAN Firewall Configuration.*

![SG-3100 / Firewall / Rules / LAN / Final](images/Firewall_Rules_Dns_Final.png)

---

## [Return](../README.md)

![WARN +](https://via.placeholder.com/15/FF6A00/000000?text=+) *For Bench Lab Only.*
![OK +](https://via.placeholder.com/15/4CFF00/000000?text=+) *For Production.*

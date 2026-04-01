# Advanced ISP Lab
Representing advanced concepts from real-world using various techologies and solutions such as MPLS, BGP Route-Reflector, Multi-VRF, and interexchange customer traffic

Here below a graphical representation of the lab

![MPLS | MBGP | Adv ISP Lab](https://github.com/user-attachments/assets/b626f261-f653-458c-9f47-3cff8f81b9c3)

- Red circle is the ISP Network
- Yellow circle is CUSTOMER C (VRF CUST-C)
- Blue circle is CUSTOMER A (VRF CUST-A)
- Green circle is CUSTOMER B (VRF CUST_B)

Underlay is managed by MBGP and OSPF protocols, while the overlay is mangaged by MPLS

Each customer is under its own VRF

The goals of this lab are:
- Build a redundant ISP core network using BGP-RR on R2 and R6 and have a full topology view using OSPF
- Using MPLS protocol to allow all customers to communicate between their own sites
- Redistribute OSPF configured on each CE customer router into the BGP in order to reach and be reached from their respective remote sites
- Allow CUSTOMER A to reach a single ip address in CUSTOMER C (for example a public server)
- Keep traffic of each customer separated by using VRF technologies

Keep in mind that some configurations are not implemented since was out of the scope of this lab

I used VirtualBox on Fedora Linux with c7200-adventerprisek9-mz.152-4.S6 image for all routers

Feel free to suggest any improvement if needed

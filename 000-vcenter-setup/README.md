# Vcenter Setup
VCenter installation

Requirements\
Domain name: minhchu.xyz
administrator@vsphere.local
@Chudeptrai123
| Host      | Ip Address | Private FQDN |
| ----------- | ----------- | ----------- |
| dns_server      | 192.168.1.200       | ns1.homelab.minhchu.xyz |
| dns_server_bacup    | 192.168.1.201       | ns2.homelab.minhchu.xyz |
| ESXi-1      | 192.168.1.9       | esxi1.homelab.minhchu.xyz |
| ESXi-2      | 192.168.1.10        | esxi2.homelab.minhchu.xyz |

![SegmentTree](./imgs/test.png)
*<p align="center"> Ví dụ về cây phân đoạn quản lý tổng của đoạn </p>*

Fix ubuntu issue
```bash
sudo groupadd promiscuous
sudo usermod -a -G promiscuous mc
sudo chgrp promiscuous /dev/vmnet*
sudo chmod g+rw /dev/vmnet*
```

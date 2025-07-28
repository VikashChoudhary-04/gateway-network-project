# 🛜 Cisco Gateway Project

This project is a *Cisco Gateway network setup* created using Cisco Packet Tracer. It demonstrates how to configure multiple routers and PCs in a network using *static routing*.

---

## 🧠 What You’ll Learn

- How to assign IP addresses to PCs and routers
- How to connect routers together
- How to configure static routes
- How to test full network connectivity using the ping command

---

## 🖥 Network Topology

The network contains:

- 3 Routers (Router8, Router9, Router10)
- 3 PCs (PC5, PC6, PC7)
- Connections between all routers and PCs
- Static routes for full connectivity

Each PC is connected to a different router, and each router knows how to reach all networks using manual routes.

---

## 🔧 IP Address Plan

| Device     | Interface        | IP Address  |
|------------|------------------|-------------|
| PC5        | FastEthernet0    | 10.0.0.2    |
| Router8    | G0/0             | 10.0.0.1    |
| Router8    | G0/1             | 10.0.3.1    |
| Router9    | G0/0             | 10.0.3.2    |
| Router9    | G0/1             | 10.0.1.1    |
| PC6        | FastEthernet0    | 10.0.1.2    |
| Router9    | G0/2             | 10.0.5.2    |
| Router10   | G0/1             | 10.0.5.1    |
| Router10   | G0/0             | 10.0.2.1    |
| PC7        | FastEthernet0    | 10.0.2.2    |

Subnet mask used: 255.255.255.0 for all

---

## ⚙ Configuration Files

See the [router-configs.txt](./router-configs.txt) file for all the commands used on each router.

---

## 🧪 How to Test the Network

1. Open the .pkt file in Cisco Packet Tracer.
2. Use the *ping* command from each PC to test others:
   - From PC5: ping 10.0.1.2, ping 10.0.2.2
   - From PC6: ping 10.0.0.2, ping 10.0.2.2
   - From PC7: ping 10.0.0.2, ping 10.0.1.2
3. You can also test ping between routers.

All pings should be successful if configuration is correct.

---

## 📂 Files in This Repo

- router-configs.txt – CLI code used for each router
- gateway.pkt – Cisco Packet Tracer file (optional)
- README.md – This file

---

## 🏁 Project Status

✅ All router and PC connections tested  
✅ All static routes configured correctly  
✅ Full connectivity verified using ping

---

## 🙋‍♂ Author

Created by Vikash Choudhary  
Made with 💻 using Cisco Packet Tracer

---

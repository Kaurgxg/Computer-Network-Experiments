# Experiment 2 -- Packet Flow Visualization Using Simulation Mode

## How to Open and Test

1. Open Cisco Packet Tracer.
2. Load the file `exp2_packetflow.pkt`.
3. Verify IP configuration on all PCs:
   - PC0 → 192.168.20.1  
   - PC1 → 192.168.20.2  
   - PC2 → 192.168.20.3  
4. Open Command Prompt on PC0.

5. Perform first ping:
```
ping 192.168.20.2
```

6. Switch to **Simulation Mode**.
7. Observe packet flow in Event List:
   - ARP Request (Broadcast)
   - ARP Reply
   - ICMP Echo Request
   - ICMP Echo Reply

8. Perform second ping:
```
ping 192.168.20.2
```

9. Observe:
   - Only ICMP packets (no ARP)
   - Faster communication due to caching

10. Check **Switch MAC Address Table**:
   - Observe learned MAC addresses
   - Verify intelligent forwarding (no unnecessary broadcast)

---

## Files Included

- exp2_packetflow.pkt (Packet Tracer file)  
- output_exp2.txt (Ping observations)  
- exp2_report.pdf (Detailed report with screenshots)  
- README.md (Instructions)  

---

## Learning Outcomes

- Understanding packet flow in a LAN  
- Observing ARP and ICMP protocols in action  
- Learning why the first ping is slower  
- Understanding MAC address learning in switches  
- Analyzing packet movement using Simulation Mode  

---

## Key Observations

### First Ping
- ARP Request broadcasted  
- ARP Reply received  
- ICMP communication initiated  
- More packets due to ARP process  

### Second Ping
- No ARP required  
- Only ICMP packets observed  
- Faster communication (MAC already cached)  

### MAC Learning
- Switch learns MAC addresses  
- Frames sent only to correct port  
- Network becomes efficient after learning  

---

## Final Result

- ARP resolves IP to MAC before communication  
- ICMP is used for data transmission  
- After caching, communication becomes faster and efficient  
- Packet flow successfully visualized using Simulation Mode

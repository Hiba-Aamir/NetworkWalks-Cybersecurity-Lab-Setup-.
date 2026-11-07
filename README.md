# NetworkWalks-Cybersecurity-Lab-Setup-.
My Cybersecurity Lab Setup files and notes

My Cybersecurity Lab Setup files and notes[cite: 6].

## Lab Steps Completed:
1. **Downloaded & Installed VirtualBox & Kali Linux.**
2. **Configured NAT Network with 10.0.0.0/24.**
3. **Set Static IP on Kali Linux:**
   - **Address:** 10.0.0.2
   - **Netmask:** 24
   - **Gateway:** 10.0.0.1
   - **DNS:** 8.8.8.8
4. **Fixed DAD Timeout Issue (Kali 2026.1+):**
   ```bash
   sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
   sudo nmcli connection down "Wired connection 1"
   sudo nmcli connection up "Wired connection 1"
   
Tested Internet And Connectivity:
Successfully pinged gateway (10.0.0.1) and Google (8.8.8.8 / google.com) with 0% packet loss.

Taken Snapshot:

"Kali Linux Network Configured" snapshot saved successfully.
<img width="1363" height="719" alt="Screenshot 2026-11-07 132632" src="https://github.com/user-attachments/assets/14c0e832-8f26-4ae5-84d1-d5f09ee37863" />



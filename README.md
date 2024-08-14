# HackMyVM - Gift

**Lab enviroment**

Kali: **10.0.2.21**

Gift: **10.0.2.20**

## 1. INFORMATION GATHERING
### a. Check IP Kali
ip a | grep /24

![ip address](/images/ip%20address.png)
### b. Netdiscover
sudo netdiscover -r 10.0.2.0/24

![netdiscover](/images/netdiscovery.png)
### c. Nmap Target Ports
sudo namp -sS 10.0.2.20

![nmap target ports](/images/nmap%20target%20port.png)
### d. Nmap Target Services
sudo nmap -sS -p 22,80 -A 10.0.2.20

![nmap target services](/images/nmap%20target%20services.png)
## 2. ENUMERATION HTTP (PORT 80/tcp)
![nmap target services](/images/enumeration%20http.png)
## 3. EXPLOITATION SSH (PORT 22/tcp)
### a. Ncrack
![ncrack](/images/exploitation%20ssh.png)

Result: username login is **root** and password is **simple**

### b. SSH Client
![ssh client](/images/ssh%20client.png)

### c. Capture The Flags
![CTF](/images/CTF.png)



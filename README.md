sina@sina-VivoBook-15-ASUS-Laptop-X542UF:~/xray-mitm$ sudo cp mycert.crt /usr/local/share/ca-certificates/mycert.crt
sudo update-ca-certificates
wget https://raw.githubusercontent.com/patterniha/MITM-DomainFronting/main/Xray-config/MITM-DomainFronting.json
./xray run -c MITM-DomainFronting.json
[sudo] password for sina:         
cp: cannot stat 'mycert.crt': No such file or directory
Updating certificates in /etc/ssl/certs...
0 added, 0 removed; done.
Running hooks in /etc/ca-certificates/update.d...
done.
--2026-06-13 12:44:01--  https://raw.githubusercontent.com/patterniha/MITM-DomainFronting/main/Xray-config/MITM-DomainFronting.json
Resolving raw.githubusercontent.com (raw.githubusercontent.com)... 185.199.110.133, 185.199.108.133, 185.199.111.133, ...
Connecting to raw.githubusercontent.com (raw.githubusercontent.com)|185.199.110.133|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9553 (9.3K) [text/plain]
Saving to: ‘MITM-DomainFronting.json’

MITM-DomainFronting 100%[===================>]   9.33K  --.-KB/s    in 0s      

2026-06-13 12:44:04 (59.4 MB/s) - ‘MITM-DomainFronting.json’ saved [9553/9553]

Xray 26.3.27 (Xray, Penetrates Everything.) d2758a0 (go1.26.1 linux/amd64)
A unified platform for anti-censorship.
2026/06/13 12:44:04.735633 [Info] infra/conf/serial: Reading config: &{Name:MITM-DomainFronting.json Format:json}
Failed to start: main: failed to load config files: [MITM-DomainFronting.json] > infra/conf: failed to build inbound config with tag tls-decrypt-h11 > infra/conf: Failed to build TLS config. > infra/conf: failed to parse certificate > open /home/sina/xray-mitm/mycert.crt: no such file or directory
sina@sina-VivoBook-15-ASUS-Laptop-X542UF:~/xray-mitm$ 


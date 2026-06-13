sudo cp mycert.crt /usr/local/share/ca-certificates/mycert.crt
sudo update-ca-certificates
wget https://raw.githubusercontent.com/patterniha/MITM-DomainFronting/main/Xray-config/MITM-DomainFronting.json
./xray run -c MITM-DomainFronting.json

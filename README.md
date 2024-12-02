# open-port-firewall-win

### OPEN

```bash

netsh advfirewall firewall add rule name="Open Port 10000 IN" protocol=TCP dir=in localport=10000 action=allow
netsh advfirewall firewall add rule name="Open Port 10000 OUT" protocol=TCP dir=out localport=10000 action=allow

```

### CLOSE

```bash

netsh advfirewall firewall delete rule name="Open Port 10000 IN" protocol=TCP dir=in localport=10000
netsh advfirewall firewall delete rule name="Open Port 10000 OUT" protocol=TCP dir=out localport=10000

```

### CHECK 

```bash
netsh advfirewall firewall show rule name="Open Port 10000 IN"
netsh advfirewall firewall show rule name="Open Port 10000 OUT"

```

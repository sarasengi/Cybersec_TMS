192.168.0.0/25
128 адресов (126 используются под хосты):<br>
```Network address: 192.168.0.0; usable range: 192.168.0.1 - 192.168.0.126; broadcast: 192.168.0.127```<br>
_Шлюзом обычно делают первый адрес из диапазона подсети_

2 подсети /26 (255.255.255.192):<br>
128/2 = 64 адреса в каждой подсети, по 62 хостовых
* ```Network address: 192.168.0.0; usable range: 192.168.0.1 - 192.168.0.62; broadcast: 192.168.0.63```
* ```Network address: 192.168.0.64; usable range: 192.168.0.65 - 192.168.0.126; broadcast: 192.168.0.127```

или 4 подсети /27 (255.255.255.224):<br>
128/4 = 32 адреса в каждой подсети, по 30 хостовых
* ```Network address: 192.168.0.0; usable range: 192.168.0.1 - 192.168.0.30; broadcast: 192.168.0.31```
* ```Network address: 192.168.0.32; usable range: 192.168.0.33 - 192.168.0.62; broadcast: 192.168.0.63```
* ```Network address: 192.168.0.64; usable range: 192.168.0.65 - 192.168.0.94; broadcast: 192.168.0.95```
* ```Network address: 192.168.0.96; usable range: 192.168.0.97 - 192.168.0.126; broadcast: 192.168.0.127```

или 8 подсетей /28 (255.255.255.240):<br>
128/8 = 16 адресов в каждой подсети, по 14 хостовых
* ```Network address: 192.168.0.0; usable range: 192.168.0.1 - 192.168.0.14; broadcast: 192.168.0.15```
* ```Network address: 192.168.0.16; usable range: 192.168.0.17 - 192.168.0.30; broadcast: 192.168.0.31```
* ```Network address: 192.168.0.32; usable range: 192.168.0.33 - 192.168.0.46; broadcast: 192.168.0.47```
* ```Network address: 192.168.0.48; usable range: 192.168.0.47 - 192.168.0.62; broadcast: 192.168.0.63```
* ```Network address: 192.168.0.64; usable range: 192.168.0.65 - 192.168.0.78; broadcast: 192.168.0.79```
* ```Network address: 192.168.0.80; usable range: 192.168.0.81 - 192.168.0.94; broadcast: 192.168.0.95```
* ```Network address: 192.168.0.96; usable range: 192.168.0.97 - 192.168.0.110; broadcast: 192.168.0.111```
* ```Network address: 192.168.0.112; usable range: 192.168.0.113 - 192.168.0.126; broadcast: 192.168.0.127```

или 16 подсетей /29 (255.255.255.248):<br>
128/16 = 8 адресов в каждой подсети, по 6 хостовых
* ```Network address: 192.168.0.0; usable range: 192.168.0.1 - 192.168.0.6; broadcast: 192.168.0.7```
* ```Network address: 192.168.0.8; usable range: 192.168.0.9 - 192.168.0.14; broadcast: 192.168.0.15```
* ```Network address: 192.168.0.16; usable range: 192.168.0.17 - 192.168.0.22; broadcast: 192.168.0.23```
* ```Network address: 192.168.0.24; usable range: 192.168.0.25 - 192.168.0.30; broadcast: 192.168.0.31```
* ```Network address: 192.168.0.32; usable range: 192.168.0.33 - 192.168.0.38; broadcast: 192.168.0.39```
* ```Network address: 192.168.0.40; usable range: 192.168.0.41 - 192.168.0.46; broadcast: 192.168.0.47```
* ```Network address: 192.168.0.48; usable range: 192.168.0.49 - 192.168.0.54; broadcast: 192.168.0.55```
* ```Network address: 192.168.0.56; usable range: 192.168.0.57 - 192.168.0.62; broadcast: 192.168.0.63```
* ```Network address: 192.168.0.64; usable range: 192.168.0.65 - 192.168.0.70; broadcast: 192.168.0.71```
* ```Network address: 192.168.0.72; usable range: 192.168.0.73 - 192.168.0.78; broadcast: 192.168.0.79```
* ```Network address: 192.168.0.80; usable range: 192.168.0.81 - 192.168.0.86; broadcast: 192.168.0.87```
* ```Network address: 192.168.0.88; usable range: 192.168.0.89 - 192.168.0.94; broadcast: 192.168.0.95```
* ```Network address: 192.168.0.96; usable range: 192.168.0.97 - 192.168.0.102; broadcast: 192.168.0.103```
* ```Network address: 192.168.0.104; usable range: 192.168.0.105 - 192.168.0.110; broadcast: 192.168.0.111```
* ```Network address: 192.168.0.112; usable range: 192.168.0.113 - 192.168.0.118; broadcast: 192.168.0.119```
* ```Network address: 192.168.0.120; usable range: 192.168.0.121 - 192.168.0.126; broadcast: 192.168.0.127```

или 32 подсетей /30 (255.255.255.252):<br>
128/32 = 4 адресов в каждой подсети, по 2 хостовых
* ```Network address: 192.168.0.0; usable range: 192.168.0.1 - 192.168.0.2; broadcast: 192.168.0.3```
* ```Network address: 192.168.0.4; usable range: 192.168.0.5 - 192.168.0.6; broadcast: 192.168.0.7```
* ```Network address: 192.168.0.8; usable range: 192.168.0.9 - 192.168.0.10; broadcast: 192.168.0.11```
* ```Network address: 192.168.0.12; usable range: 192.168.0.13 - 192.168.0.14; broadcast: 192.168.0.15```
* ```Network address: 192.168.0.16; usable range: 192.168.0.17 - 192.168.0.18; broadcast: 192.168.0.19```
* ```Network address: 192.168.0.20; usable range: 192.168.0.21 - 192.168.0.22; broadcast: 192.168.0.23```
* ```Network address: 192.168.0.24; usable range: 192.168.0.25 - 192.168.0.26; broadcast: 192.168.0.27```
* ```Network address: 192.168.0.28; usable range: 192.168.0.29 - 192.168.0.30; broadcast: 192.168.0.31```
* ```Network address: 192.168.0.32; usable range: 192.168.0.33 - 192.168.0.34; broadcast: 192.168.0.35```
* ```Network address: 192.168.0.36; usable range: 192.168.0.37 - 192.168.0.38; broadcast: 192.168.0.39```
* ```Network address: 192.168.0.40; usable range: 192.168.0.41 - 192.168.0.42; broadcast: 192.168.0.43```
* ```Network address: 192.168.0.44; usable range: 192.168.0.45 - 192.168.0.46; broadcast: 192.168.0.47```
* ```Network address: 192.168.0.48; usable range: 192.168.0.49 - 192.168.0.50; broadcast: 192.168.0.51```
* ```Network address: 192.168.0.52; usable range: 192.168.0.53 - 192.168.0.54; broadcast: 192.168.0.55```
* ```Network address: 192.168.0.56; usable range: 192.168.0.57 - 192.168.0.58; broadcast: 192.168.0.59```
* ```Network address: 192.168.0.60; usable range: 192.168.0.61 - 192.168.0.62; broadcast: 192.168.0.63```
* ```Network address: 192.168.0.64; usable range: 192.168.0.65 - 192.168.0.66; broadcast: 192.168.0.67```
* ```Network address: 192.168.0.68; usable range: 192.168.0.69 - 192.168.0.70; broadcast: 192.168.0.71```
* ```Network address: 192.168.0.72; usable range: 192.168.0.73 - 192.168.0.74; broadcast: 192.168.0.75```
* ```Network address: 192.168.0.76; usable range: 192.168.0.77 - 192.168.0.78; broadcast: 192.168.0.79```
* ```Network address: 192.168.0.80; usable range: 192.168.0.81 - 192.168.0.82; broadcast: 192.168.0.83```
* ```Network address: 192.168.0.84; usable range: 192.168.0.85 - 192.168.0.86; broadcast: 192.168.0.87```
* ```Network address: 192.168.0.88; usable range: 192.168.0.89 - 192.168.0.90; broadcast: 192.168.0.91```
* ```Network address: 192.168.0.92; usable range: 192.168.0.93 - 192.168.0.94; broadcast: 192.168.0.95```
* ```Network address: 192.168.0.96; usable range: 192.168.0.97 - 192.168.0.98; broadcast: 192.168.0.99```
* ```Network address: 192.168.0.100; usable range: 192.168.0.101 - 192.168.0.102; broadcast: 192.168.0.103```
* ```Network address: 192.168.0.104; usable range: 192.168.0.105 - 192.168.0.106; broadcast: 192.168.0.107```
* ```Network address: 192.168.0.108; usable range: 192.168.0.109 - 192.168.0.110; broadcast: 192.168.0.111```
* ```Network address: 192.168.0.112; usable range: 192.168.0.113 - 192.168.0.114; broadcast: 192.168.0.115```
* ```Network address: 192.168.0.116; usable range: 192.168.0.117 - 192.168.0.118; broadcast: 192.168.0.119```
* ```Network address: 192.168.0.120; usable range: 192.168.0.121 - 192.168.0.122; broadcast: 192.168.0.123```
* ```Network address: 192.168.0.124; usable range: 192.168.0.125 - 192.168.0.126; broadcast: 192.168.0.127```

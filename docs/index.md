# **AS208223 | fOxO Internet Service Provider**
## IP Range
- `2a0e:8f02:f03d::/48`
- `2a0e:b107:1a30::/44`
- `2a06:1287:3900::/40`
- `2a12:3fc2:df00::/40`

## PoPs Location
 - 台灣台北 | Taipei, Taiwan
 - 日本東京 | Tokyo, Japan
 - 香港 | Hong Kong
 - 新加坡 | Singapore
 - 美國西雅圖 | Seattle, United States of America
 - 美國聖荷西 | San Jose, United States of America
 - 德國法蘭克福 | Frankfurt, Germany
 - 荷蘭阿姆斯特丹 | Amsterdam, Netherlands

## Edge
| Name | Location | Core | NAT64 | Anycast | Speedtest | Prefix | 
| --- | --- | --- | --- | --- | --- | --- |
| TPE Home | TW-TPE1 | ✔ | ✘ | ✘ | ✘ | `2a0e:8f02:f03d::/48`
| TPE NTHU | TW-TPE2 | ✘ | ✔ | ✔ | ✔ | `2a12:3fc2:dfaa::/48`  
| TPE Poema IX | TW-TPE3 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfdb::/48`  
| TPE AWS | TW-TPE4 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfd5::/48`  
| JP Oracle | JP-OSA1  | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfdf::/48` 
| JP Vultr | JP-TYO1  | ✘ | ✘ | ✔ | ✘ |  `2a12:3fc2:dfdc::/48`
| HK Yxvm | HK-HKG1  | ✔ | ✘ | ✔ | ✔ |  `2a12:3fc2:dfde::/48`
| HK HAT | HK-HKG2 | ✘ | ✔ | ✔ | ✘ |  `2a12:3fc2:dfdd::/48`
| SG Oracle | SG-SIN1 | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfd9::/48` 
| CN Computer CGO | CN-CGO1 | ✘ | ✘ | ✘ | ✔ |  `2a12:3fc2:dfd7::/48`
| US MOE-IX SEA | US-SEA1  | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfd8::/48`  
| DE AWS | DE-FRA1 | ✔ | ✘ | ✔ | ✔ |  `2a12:3fc2:dfda::/48`  
| NL Zero IX | NL-AMS1 |  ✘ | ✔ | ✔ | ✔ |  `2a12:3fc2:dfd4::/48`  
| US Zero IX | US-SJC1  | ✘ | ✘ | ✔ | ✘ | `2a12:3fc2:dfd6::/48`

## Anycast
#### IP Range
- `2a0e:b107:1a3b::/48`
- [Test with ping.pe](https://ping6.ping.pe/2a0e:b107:1a3b::)

## NAT64
#### Info
- Anycast
- IPv4 PoP is wgcf
#### IP Range
- `2a0e:b107:1a3b:dead:9999:9999::/96`
#### DNS64
- `2a0e:b107:1a3b:dead:9999::beef`

## Art
- `traceroute -q1 -N32 -w1 art.as208223.eu.org`

```
traceroute to art.as208223.eu.org (2a12:3fc2:dfd9:dead:1337:6666:0:ffff), 30 hops max, 80 byte packets
 1  lg.gateway.sg-sin1.as208223.eu.org (2a12:3fc2:dfd9:dead:1::1)  0.062 ms
 2  o------------------88------------------o (2a12:3fc2:dfd9:dead:1337:6666:0:1)  5.487 ms
 3  o-----------------8888-----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:2)  8.242 ms
 4  o----------------888888----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:3)  16.096 ms
 5  o---------------88888888---------------o (2a12:3fc2:dfd9:dead:1337:6666:0:4)  28.522 ms
 6  o--------------8888888888--------------o (2a12:3fc2:dfd9:dead:1337:6666:0:5)  34.524 ms
 7  o------------88888888888888------------o (2a12:3fc2:dfd9:dead:1337:6666:0:6)  40.273 ms
 8  o----------------888888----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:7)  47.938 ms
 9  o--------------8888888888--------------o (2a12:3fc2:dfd9:dead:1337:6666:0:8)  58.674 ms
10  o------------88888888888888------------o (2a12:3fc2:dfd9:dead:1337:6666:0:9)  67.179 ms
11  o----------888888888888888888----------o (2a12:3fc2:dfd9:dead:1337:6666:0:10)  74.714 ms
12  o--------8888888888888888888888--------o (2a12:3fc2:dfd9:dead:1337:6666:0:11)  84.252 ms
13  o------------88888888888888------------o (2a12:3fc2:dfd9:dead:1337:6666:0:12)  87.839 ms
14  o---------88888888888888888888---------o (2a12:3fc2:dfd9:dead:1337:6666:0:13)  95.138 ms
15  o------88888888888888888888888888------o (2a12:3fc2:dfd9:dead:1337:6666:0:14)  103.130 ms
16  o---88888888888888888888888888888888---o (2a12:3fc2:dfd9:dead:1337:6666:0:15)  110.599 ms
17  o88888888888888--8888888--8888888888888o (2a12:3fc2:dfd9:dead:1337:6666:0:16)  118.779 ms
18  o-----------------8888-----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:17)  129.343 ms
19  o-----------------8888-----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:18)  132.041 ms
20  EOF (2a12:3fc2:dfd9:dead:1337:6666:0:ffff)  141.533 ms
```

## Special Thanks
| Name | Reason | 
| --- | --- |
| AS138211 MoeQing Network Service | Free transit in US Seattle  & Singapore <br> Free VM in US Seattle <br> Free computer
| AS203314 Hats Network | Free VM & Transit in Hong Kong |
| AS140731 TOHU Public Internet | Free transit in Hong Kong & San Jose & Amsterdam
| AS138517 KSKB | Free VM in Poema IX  
| AS57406 Zero Distance LLC | Free VM in Zero IX SJC & Zero IX AMS 
| AS61302 HUIZE LTD | Free VM 
| AS202888 ZH NETWORK LIMITED | Free IPv6 Prefix /40
| AS212895 Route64 |  Free transit in Germany

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
 - 德國法蘭克福 | Frankfurt, Germany  

## Edge
| Name | Location | Core | NAT64 | Anycast | Speedtest | Prefix | 
| --- | --- | --- | --- | --- | --- | --- |
| TPE Home | TW-TPE1 | ✔ | ✘ | ✘ | ✘ | `2a0e:8f02:f03d::/48`
| TPE NTHU | TW-TPE2 | ✘ | ✔ | ✔ | ✔ | `2a12:3fc2:dfaa::/48`  
| TPE KSKB-IX | TW-TPE3 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfdb::/48`  
| JP Oracle | JP-OSA1  | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfdf::/48` 
| JP Vultr | JP-TYO1  | ✘ | ✘ | ✔ | ✘ |  `2a12:3fc2:dfdc::/48`
| HK Yxvm | HK-HKG1  | ✔ | ✘ | ✔ | ✔ |  `2a12:3fc2:dfde::/48`
| SG Oracle | SG-SIN1 | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfd9::/48` 
| CN TOHU-IX | CN-CAN1 | ✘ | ✘ | ✘ | ✔ |  `2a12:3fc2:dfdd::/48`
| CN MOE-IX CGO | CN-CGO1 | ✘ | ✘ | ✘ | ✔ |  `2a12:3fc2:dfd7::/48`
| DE Euserv | DE-FRA1 | ✔ | ✘ | ✔ | ✔ |  `2a12:3fc2:dfda::/48`  
| US MOE-IX SEA | US-SEA1  | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfd8::/48`  
| US MOE-IX DAL | US-DAL1  | ✘ | ✘ | ✔ | ✘ | `2a12:3fc2:dfd6::/48`  

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
 1  lg.gateway.sg-sin1.as208223.eu.org (2a12:3fc2:dfd9:dead:1::1)  0.068 ms
 2  o-----------------88-------------------o (2a12:3fc2:dfd9:dead:1337:6666:0:1)  3.004 ms
 3  o----------------8888------------------o (2a12:3fc2:dfd9:dead:1337:6666:0:2)  11.496 ms
 4  o----------------8888------------------o (2a12:3fc2:dfd9:dead:1337:6666:0:3)  17.889 ms
 5  o-------------8888888888---------------o (2a12:3fc2:dfd9:dead:1337:6666:0:4)  20.420 ms
 6  o------------8888888888888-------------o (2a12:3fc2:dfd9:dead:1337:6666:0:5)  26.779 ms
 7  o---------888888888888888888-----------o (2a12:3fc2:dfd9:dead:1337:6666:0:6)  29.072 ms
 8  o-------------8888888888---------------o (2a12:3fc2:dfd9:dead:1337:6666:0:7)  38.629 ms
 9  o-----------88888888888888-------------o (2a12:3fc2:dfd9:dead:1337:6666:0:8)  40.946 ms
10  o---------888888888888888888-----------o (2a12:3fc2:dfd9:dead:1337:6666:0:9)  47.324 ms
11  o-------8888888888888888888888---------o (2a12:3fc2:dfd9:dead:1337:6666:0:10)  53.872 ms
12  o----8888888888888888888888888888------o (2a12:3fc2:dfd9:dead:1337:6666:0:11)  56.137 ms
13  o-----------888888888888888------------o (2a12:3fc2:dfd9:dead:1337:6666:0:12)  62.520 ms
14  o-------888888888888888888888888-------o (2a12:3fc2:dfd9:dead:1337:6666:0:13)  64.923 ms
15  o-----8888888888888888888888888888-----o (2a12:3fc2:dfd9:dead:1337:6666:0:14)  71.654 ms
16  o--8888888888888888888888888888888888--o (2a12:3fc2:dfd9:dead:1337:6666:0:15)  81.838 ms
17  o88888888888888--8888888--8888888888888o (2a12:3fc2:dfd9:dead:1337:6666:0:16)  84.349 ms
18  o-----------------88888----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:17)  90.718 ms
19  o-----------------88888----------------o (2a12:3fc2:dfd9:dead:1337:6666:0:18)  97.644 ms
20  EOF (2a12:3fc2:dfd9:dead:1337:6666:0:ffff)  100.581 ms
```

## Special Thanks
| Name | Reason | 
| --- | --- |
| AS140731 TOHU Public Internet | Free transit in Hong Kong & Singapore <br> Free VM in TOHU-IX 
| AS138211 MoeQing Network Service | Free transit in Seattle <br> Free VM in MOE-IX 
| AS138517 KSKB | Free VM in Poema-IX  
| AS202888 ZH NETWORK LIMITED | Free IPv6 Prefix /40
| AS212895 Route64 |  Free transit in Germany

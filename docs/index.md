# **AS208223 | fOxO Internet Service Provider**
## IP Range
- `160.25.104.0/23`
- `2401:af20::/32`
- `2a0e:8f02:f03d::/48`
- `2a0e:b107:1a30::/44`
- `2602:f9f6:410::/44`
- `2a12:3fc2:df00::/40`

## PoPs Location
### IPv4
 - 台灣台北 | Taipei, Taiwan
 - 日本東京 | Tokyo, Japan
 - 加拿大溫哥華 | Vancouver, Canada

### IPv6
 - 台灣台北 | Taipei, Taiwan
 - 日本東京 | Tokyo, Japan
 - 香港 | Hong Kong
 - 加拿大溫哥華 | Vancouver, Canada
 - 新加坡 | Singapore
 - 美國弗里蒙特 | Fremont, United States of America
 - 美國堪薩斯 | Kansas, United States of America
 - 德國法蘭克福 | Frankfurt, Germany

<!-- - 美國西雅圖 | Seattle, United States of America-->


## Edge
| Name | Location | Core | NAT64 | Anycast | Speedtest | Prefix | 
| --- | --- | --- | --- | --- | --- | --- |
| TW Home | TW-TPE1 | ✔ | ✘ | ✘ | ✘ | `2a0e:8f02:f03d::/48`
| TW NTHU | TW-TPE2 | ✘ | ✔ | ✘ | ✘ | `2a12:3fc2:dfaa::/48`  
| TW Poema IX | TW-TPE3 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfdb::/48`  
| TW STUIX | TW-TPE5 | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfd2::/48`
| TW FCU | TW-TXG1 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfce::/48`
| JP Oracle | JP-OSA1  | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfdf::/48` 
| JP Vultr | JP-TYO1  | ✘ | ✘ | ✔ | ✘ |  `2a12:3fc2:dfdc::/48`
| HK MDIX |  HK-HKG1 | ✘ | ✘ | ✘ | ✘ |  `2401:af20:dfd7::/48` 
| HK DMIT |  HK-HKG2 | ✘ | ✘ | ✘ | ✘ |  `2a12:3fc2:dfdd::/48` 
| HK MDIX | HK-HKG4 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfcd::/48`  
| CN Spark VM | CN-SZX1 | ✘ | ✘ | ✘ | ✘ |  `2401:af20:dfd0::/48`
| CN AKIX TFU | CN-TFU1 | ✘ | ✘ | ✘ | ✘ |  `2a12:3fc2:dfd3::/48`
| SG Oracle | SG-SIN1 | ✔ | ✔ | ✔ | ✔ | `2a12:3fc2:dfd9::/48` 
| SG MDIX | SG-SIN2 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfcc::/48`
| CA Unmetered.Exchange | CA-YVR1 | ✔ | ✔ | ✔ | ✔ |  `2a12:3fc2:dfde::/48`
| CA Home | CA-YVR2| ✔ | ✘ | ✘ | ✘ | `2401:af20:f03d::/48`
| US Zero IX | US-SJC1  | ✘ | ✘ | ✔ | ✘ | `2a12:3fc2:dfd6::/48`
| US Kawaii MCI | US-MCI1  | ✘ | ✔ | ✔ | ✘ | `2a12:3fc2:dfd8::/48` 
| US NHIX MCI | US-MCI2  | ✘ | ✘ | ✔ | ✘ | `2a12:3fc2:dfca::/48` 
| DE TMW-IX | DE-FRA2 | ✘ | ✔ | ✔ | ✘ | `2a12:3fc2:dfd4::/48`


<!-- 
| TW AWS | TW-TPE4 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfd5::/48`  
| TW NTU | TW-TPE-6 | ✘ | ✘ | ✘ | ✘ | `2a12:3fc2:dfcb::/48`
| DE AWS | DE-FRA1 | ✔ | ✘ | ✘ | ✔ |  `2a12:3fc2:dfda::/48`  
| HK AWS | HK-HKG3 | ✘ | ✘ | ✘ | ✘ |  `2a12:3fc2:dfcf::/48`
| HK Skywolf | HK-HKG1  | ✔ | ✘ | ✔ | ✔ |  `2a12:3fc2:dfde::/48`
| US AWS | US-SEA2  | ✔ | ✔ | ✔ | ✘ | `2a12:3fc2:dfd1::/48`
| KR AWS| KR-ICN1 | ✘ | ✘ | ✘ | ✘ |  `2a12:3fc2:dfd0::/48`
| US Vultr ORD | US-ORD1  | ✘ | ✔ | ✔ | ✘ | `2a12:3fc2:dfd8::/48`  
-->

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
- [Test with ping.pe](https://ping6.ping.pe/2a0e:b107:1a3b:dead:9999:9999:101:101)

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
| AS18041 Taiwan Digital Streaming |  Free IPv4 & IPv6 transit in Taipei
| AS44324 MoeDove | Free transit in Hong Kong & Singapore & America & Taiwan  <br> Free VM in Singapore & Hong Kong
| AS215828 TMW Global Networks | Free transit in Frankfurt <br>  Free VM in TMW-IX
| AS27523 Kawaii Networks | Free transit in America <br> Free VM in America
| AS216324 Hyper Group Network Ltd | Free transit in America <br> Free VM in HNIX
| AS57406 Zero Distance LLC | Free VM in Zero IX SJC
| AS138517 KSKB | Free VM in Poema IX  
| AS213605 Pysio NetWork | Free VM in AKIX  
| <del>AS202888 ZH NETWORK LIMITED (Archived)</del> <br> AS210000 DAOport Internet Infrastructure | Free IPv6 Prefix /40
| AS138211 MoeQing Network Service |  Free IPv6 Prefix /44
| AS6939 Hurricane Electric |  Free transit in Taipei & Canada
| AS41051 Openfactory GmbH | ASN registry & Free transit in Germany
| AS212895 Route64 |  Free transit in Germany
| Spark VM | Free IEPL VM in Shenzhen to Hong Kong


<!-- 
| AS203314 Hats Network | Free VM & Transit in Hong Kong | 
| AS215364 Infinitron Internet LLC | Free transit in Hong Kong <br> Free VM in JJIX
| AS140731 TOHU Public Internet | Free transit in Hong Kong

-->

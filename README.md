# V2RayAggregator

[![Collect](https://github.com/SSgumS/V2RayAggregator/actions/workflows/Collector.yml/badge.svg)](https://github.com/SSgumS/V2RayAggregator/actions/workflows/Collector.yml) [![Airport Collect](https://github.com/SSgumS/V2RayAggregator/actions/workflows/Airport_Collector.yml/badge.svg)](https://github.com/SSgumS/V2RayAggregator/actions/workflows/Airport_Collector.yml)

## Quick Note & Updates

🔴 ~~This project is still under maintance. so don't use it until further announcement cause there is a chance you will get errors while updating the nodes, etc.~~

🟢 11/1/2022: from now you can use this project. also readme file updated with the recent changes so you can find out which file to use.

## Introduction

The automation functions of this repository are all implemented based on `GitHub Actions`

Test the speed of each free node pool on the network and the nodes shared by bloggers to screen out relatively stable and high-speed nodes, and then import them into the warehouse for sharing records.

The speed measurement function is implemented in the `GitHub Actions` environment using [LiteSpeedTest](https://github.com/xxf098/LiteSpeedTest), so there are many nodes in the United States, which cannot well represent the node availability in the domestic network environment.

## Features

-   Lots of sources 😯
-   Remove all duplicate nodes 🤤
-   Providing nodes in major formats (YAML, clash, v2ray, base64) 🦋
-   No additional conversion to prevent breaking the nodes 🌿
-   Filtering best nodes by testing them and sorting them based on their average speed 🍀

## Recent Todos

-   [x] ~~Fix region based lite speed test (mainly EU)~~ 👀
-   [x] Fix Sort Based on the Avg Speed 👀
-   [x] Update required softwares to latest version 👀
-   [x] Fix sources that subconvertor unable to convert 👀
-   [x] Add separate files & functions for airport 👀
-   [x] Fix name (emoji+ip) for all log files 👀
-   [x] Separate sub list for airports & other nodes 👀
-   [x] Fixed clash template 👀
-   [ ] Cleanup redundant files and functions (dev Branch) 🧲

## Visualizer

-   Log Visualizer on Netlify
    > if you click on any node url it will copy to clipboard

|              |                                                                   Link to Log                                                                    |
| :----------: | :----------------------------------------------------------------------------------------------------------------------------------------------: |
| Public Nodes |       <a href="https://55292969231427515295.netlify.app/" target="_blank"><img src="https://i.ibb.co/g32RmJy/netlify.png" width="35"/></a>       |
|   Airport    | <a href="https://55292969231427515295.netlify.app?type=airport" target="_blank"><img src="https://i.ibb.co/g32RmJy/netlify.png" width="35"/></a> |

## Instructions & Usage

### Tips

-   If you see an IP repeated more than once it's usually because of the different ports.
-   (Group 2) Some free airports only provide 1GB of traffic or have limited time to use that's why I update the airport node every 2 hours. so if you want to use them set the auto-update option on your client to get fresh nodes.
-   (Group 1) Other public nodes are more stable and will be updated every 12 hours.
-   Depending on your internet provider and location, some nodes might not work.

### Ready to import (200 filtered nodes)

> Just import the following subscription link into the corresponding client. Use a client that atleast support ss + ssr + vmess + trojan.

Nodes filtered using speedtest measurement will be stored in following files:

-   Group 1 (Contains free public nodes)

*   [Base64](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/Eternity)
*   [Mixed](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/Eternity.txt)
*   [Clash](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/Eternity.yml)

-   Group 2 (Contains only free airports)

*   [Base64](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/EternityAir)
*   [Mixed](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/EternityAir.txt)
*   [Clash](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/EternityAir.yml)

### For Local Testing (all nodes)

> Only for local testing because the number of nodes is too high and your client will crash if you import them

All of the nodes merged together will be stored in following files:

-   Group 1 (Contains free public nodes)

*   [Base64](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/sub_merge_base64.txt)
*   [Mixed](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/sub_merge.txt)
*   [Clash](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/sub_merge_yaml.yml)

-   Group 2 (Contains only free airports)

*   [Base64](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/airport_merge_base64.txt)
*   [Mixed](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/airport_sub_merge.txt)
*   [Clash](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/airport_merge_yaml.yml)

### Manual Subs Conversion

-   If your client does not support the formats that provided here use below services to convert them to your client format (like surfboard)
    > Services for online sub conversion:
-   [sub-web-modify](https://sub.v1.mk/)
-   [bianyuan](https://bianyuan.xyz/)

-   **If you don't like the groups and rules that are already set, you can simply use bianyuan API like this::**
    > don't use this API for your personal airport subs! Pls run the subconverter locally

```
https://pub-api-1.bianyuan.xyz/sub?target=(OutputFormat)&url=(SubUrl)&insert=false

For Example:
(OutputFormat) = clash
(SubUrl) = https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/Eternity.yml

https://pub-api-1.bianyuan.xyz/sub?target=clash&url=https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/Eternity.yml&insert=false

Now you can use the link above to import the subs into your client
```

<br/>

## Node Information

### high-speed node
high-speed node quantity: `200`
high-speed node quantity: `200`

<details>
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@37.19.198.160:443#%F0%9F%87%BA%F0%9F%87%B8US-37.19.198.160-0062
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@37.19.198.243:443#%F0%9F%87%BA%F0%9F%87%B8US-37.19.198.243-0068
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@37.19.198.236:443#%F0%9F%87%BA%F0%9F%87%B8US-37.19.198.236-0070
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@37.19.198.244:443#%F0%9F%87%BA%F0%9F%87%B8US-37.19.198.244-0069
    trojan://NQ26071394@thankful-piranha.rooster465.autos:443?security=tls&sni=thankful-piranha.rooster465.autos#%F0%9F%87%AE%F0%9F%87%AAIE-3.255.100.31-0100
    trojan://NQ26071394@funky-opossum.rooster465.autos:443?security=tls&sni=funky-opossum.rooster465.autos#%F0%9F%87%AE%F0%9F%87%AAIE-108.131.117.154-0090
    trojan://OD90375861@wired-tick.rooster465.autos:443?security=tls#%F0%9F%87%AE%F0%9F%87%AAIE-52.212.156.233-0079
    trojan://NQ26071394@correct-starfish.rooster465.autos:443?security=tls&sni=correct-starfish.rooster465.autos#%F0%9F%87%AE%F0%9F%87%AAIE-34.249.41.208-0078
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.218:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.218-6054
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.179:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.179-0084
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.186:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.186-0093
    trojan://NQ26071394@fun-labrador.rooster465.autos:443?security=tls&sni=fun-labrador.rooster465.autos#%F0%9F%87%AE%F0%9F%87%AAIE-34.242.69.173-0081
    trojan://CF68213490@tolerant-rattler.rooster465.autos:443?security=tls#%F0%9F%87%BA%F0%9F%87%B8US-54.245.167.246-6019
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@82.38.31.155:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.155-0099
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@82.38.31.34:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.34-5891
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.189:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.189-0085
    trojan://CF68213490@polite-coyote.rooster465.autos:443?security=tls&sni=polite-coyote.rooster465.autos#%F0%9F%87%BA%F0%9F%87%B8US-44.251.239.102-0066
    ss://cmM0LW1kNToxNGZGUHJiZXpFM0hEWnpzTU9yNg==@146.70.61.37:8080#%F0%9F%87%AC%F0%9F%87%A7GB-146.70.61.37-0088
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@82.38.31.16:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.16-0097
    trojan://HW85960347@dashing-possum.rooster465.autos:443?security=tls&sni=dashing-possum.rooster465.autos#%F0%9F%87%BA%F0%9F%87%B8US-34.219.189.213-0402
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.187:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.187-0096
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.210:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.210-0073
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.214:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.214-0080
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.202:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.202-0087
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@193.29.139.151:8080#%F0%9F%87%B3%F0%9F%87%B1NL-193.29.139.151-0098
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@82.38.31.57:443#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.57-0095
    trojan://KV63147582@wondrous-dogfish.rooster465.autos:443?security=tls&sni=wondrous-dogfish.rooster465.autos#%F0%9F%87%BA%F0%9F%87%B8US-35.91.0.206-3093
    trojan://NQ26071394@ready-kangaroo.rooster465.autos:443?security=tls&sni=ready-kangaroo.rooster465.autos#%F0%9F%87%AB%F0%9F%87%B7FR-35.181.65.111-0101
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@193.29.139.235:8080#%F0%9F%87%B3%F0%9F%87%B1NL-193.29.139.235-0092
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@82.38.31.149:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.149-0076
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.184:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.184-6055
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.192:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.192-0083
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@156.146.38.168:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.168-0065
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@193.29.139.204:8080#%F0%9F%87%B3%F0%9F%87%B1NL-193.29.139.204-0086
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.208:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.208-0094
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.191:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.191-0077
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@156.146.38.167:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.167-0061
    trojan://NQ26071394@quiet-condor.rooster465.autos:443?security=tls#%F0%9F%87%A9%F0%9F%87%AADE-63.178.193.196-6044
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvWklvQTY5UTh5aGNRVjhrYTNQYTNB@82.38.31.15:443#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.15-0089
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@156.146.38.169:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.169-0064
    trojan://OD90375861@busy-hermit.rooster465.autos:443?security=tls&sni=busy-hermit.rooster465.autos#%F0%9F%87%A9%F0%9F%87%AADE-3.67.171.41-0105
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@156.146.38.170:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.170-0063
    trojan://CF68213490@harmless-lab.rooster465.autos:443?security=tls&sni=harmless-lab.rooster465.autos#%F0%9F%87%A9%F0%9F%87%AADE-18.184.4.15-0149
    trojan://KV63147582@evolving-baboon.rooster465.autos:443?security=tls&sni=evolving-baboon.rooster465.autos#%F0%9F%87%A9%F0%9F%87%AADE-3.76.41.23-0111
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHNXA2d3c0bzY3SEI=@108.181.118.10:8388#%F0%9F%87%A8%F0%9F%87%A6CA-108.181.118.10-0082
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@109.201.152.181:443#%F0%9F%87%B3%F0%9F%87%B1NL-109.201.152.181-0072
    trojan://XG59623478@enabling-asp.rooster465.autos:443?security=tls&sni=enabling-asp.rooster465.autos#%F0%9F%87%A9%F0%9F%87%AADE-18.195.11.206-0103
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHNXA2d3c0bzY3SEI=@108.181.0.177:8388#%F0%9F%87%BA%F0%9F%87%B8US-108.181.0.177-0071
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTprMWRCT21PQjRvcWk3VW1wMzdhMWJR@82.38.31.205:8080#%F0%9F%87%AC%F0%9F%87%A7GB-82.38.31.205-0075
    trojan://NQ26071394@grateful-bedbug.rooster465.autos:443?security=tls&sni=grateful-bedbug.rooster465.autos#%F0%9F%87%B3%F0%9F%87%B1NL-89.39.70.85-0109
    trojan://NQ26071394@kind-unicorn.rooster465.autos:443?security=tls&sni=kind-unicorn.rooster465.autos#%F0%9F%87%B5%F0%9F%87%B1PL-62.112.222.177-0136
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@173.244.56.6:443#%F0%9F%87%BA%F0%9F%87%B8US-173.244.56.6-0102
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@173.244.56.9:443#%F0%9F%87%BA%F0%9F%87%B8US-173.244.56.9-0106
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpDSm1UQ0N4N0x0dWQ=@108.181.58.239:8388#%F0%9F%87%B3%F0%9F%87%B1NL-108.181.58.239-0187
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpDSm1UQ0N4N0x0dWQ=@108.181.126.122:8388#%F0%9F%87%B3%F0%9F%87%B1NL-108.181.126.122-0189
    trojan://CF68213490@emerging-weevil.rooster465.autos:443?security=tls#%F0%9F%87%B5%F0%9F%87%B1PL-62.112.222.151-5917
    trojan://KV63147582@more-trout.rooster465.autos:443?security=tls&sni=more-trout.rooster465.autos#%F0%9F%87%B5%F0%9F%87%B1PL-62.112.222.212-0110
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNToxaGhycXJva2ozYWc=@209.46.102.22:8388#%F0%9F%87%A9%F0%9F%87%AADE-209.46.102.22-0202
    trojan://CF68213490@rested-osprey.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.207.214-0146
    vmess://ewogICAgImFkZCI6ICI0NS43Ni4yMDIuNDUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjA3MWE4YTcxLWM2NTYtNGZiNi1hOTA4LTRlNDJlYjcyMjQzZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9saWtzdXpjcCIsCiAgICAicG9ydCI6IDQwMTAsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC00NS43Ni4yMDIuNDUtNjA4OCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://CF68213490@concrete-aardvark.rooster465.autos:443?security=tls&sni=concrete-aardvark.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.176.53.202-0144
    trojan://CF68213490@shining-piranha.rooster465.autos:443?security=tls&sni=shining-piranha.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.177.140.248-0176
    trojan://CF68213490@immune-mullet.rooster465.autos:443?security=tls&sni=immune-mullet.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.178.7.201-0159
    trojan://CF68213490@smashing-fawn.rooster465.autos:443?security=tls&sni=smashing-fawn.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-3.112.212.133-0133
    trojan://NQ26071394@real-ewe.rooster465.autos:443?security=tls&sni=real-ewe.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.238.178.157-0175
    trojan://NQ26071394@inviting-rabbit.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-52.194.191.229-5929
    trojan://NQ26071394@grand-grub.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-52.196.115.139-5927
    trojan://NQ26071394@firm-krill.rooster465.autos:443?security=tls&sni=firm-krill.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.199.79.137-0126
    trojan://NQ26071394@optimal-penguin.rooster465.autos:443?security=tls&sni=optimal-penguin.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.181.211.197-0143
    trojan://NQ26071394@hot-tapir.rooster465.autos:443?security=tls&sni=hot-tapir.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.230.239.115-0156
    trojan://CF68213490@steady-prawn.rooster465.autos:443?security=tls&sni=steady-prawn.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.215.200-0178
    trojan://NQ26071394@working-tomcat.rooster465.autos:443?security=tls&sni=working-tomcat.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.145.254-0147
    trojan://NQ26071394@brief-hare.rooster465.autos:443?security=tls&sni=brief-hare.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.230.244.23-0134
    trojan://NQ26071394@new-eagle.rooster465.autos:443?security=tls&sni=new-eagle.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.248.151.227-0123
    trojan://CF68213490@welcome-monitor.rooster465.autos:443?security=tls&sni=welcome-monitor.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.68.237.45-0122
    trojan://CF68213490@eternal-woodcock.rooster465.autos:443?security=tls&sni=eternal-woodcock.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.168.65.98-0206
    trojan://CF68213490@ultimate-jaguar.rooster465.autos:443?security=tls&sni=ultimate-jaguar.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.122.159-0250
    trojan://CF68213490@smooth-hornet.rooster465.autos:443?security=tls&sni=smooth-hornet.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.183.172.225-0124
    trojan://CF68213490@sincere-crappie.rooster465.autos:443?security=tls&sni=sincere-crappie.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.181.201.45-0112
    trojan://CF68213490@innocent-rattler.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-54.238.124.150-0154
    trojan://JA96378052@52.195.11.84:443?security=tls&sni=WangCai.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.11.84-0401
    trojan://CF68213490@star-moray.rooster465.autos:443?security=tls&sni=star-moray.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-3.112.149.206-0185
    trojan://CF68213490@52.195.207.214:443?security=tls&sni=rested-osprey.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.207.214-0130
    trojan://CF68213490@summary-firefly.rooster465.autos:443?security=tls&sni=summary-firefly.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.231.188.13-0171
    trojan://CF68213490@43.207.117.135:443?security=tls&sni=eminent-panther.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.117.135-0166
    trojan://CF68213490@eternal-perch.rooster465.autos:443?security=tls&sni=eternal-perch.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.183.224.87-0167
    trojan://NQ26071394@infinite-killdeer.rooster465.autos:443?security=tls&sni=infinite-killdeer.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-3.113.11.248-0152
    trojan://CF68213490@eminent-dogfish.rooster465.autos:443?security=tls&sni=eminent-dogfish.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.153.3-0170
    trojan://CF68213490@live-drake.rooster465.autos:443?security=tls&sni=live-drake.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.107.39-0160
    trojan://CF68213490@thankful-mustang.rooster465.autos:443?security=tls&sni=thankful-mustang.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.199.23.158-0121
    trojan://CF68213490@sacred-anemone.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-13.230.252.28-0135
    trojan://CF68213490@settling-humpback.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-13.112.180.140-0151
    trojan://NQ26071394@fit-marten.rooster465.autos:443?security=tls&sni=fit-marten.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.249.164.14-0188
    trojan://CF68213490@upright-rhino.rooster465.autos:443?security=tls&sni=upright-rhino.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-3.112.231.253-0145
    trojan://CF68213490@darling-mongrel.rooster465.autos:443?security=tls&sni=darling-mongrel.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.238.160.68-0174
    trojan://CF68213490@adapting-basilisk.rooster465.autos:443?security=tls&sni=adapting-basilisk.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.250.235.241-0173
    trojan://CF68213490@star-cheetah.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-18.183.215.94-0114
    trojan://CF68213490@in-oriole.rooster465.autos:443?security=tls&sni=in-oriole.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.198.88.225-0214
    trojan://HW85960347@ultimate-cardinal.rooster465.autos:443?security=tls&sni=ultimate-cardinal.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.208.29-3094
    trojan://CF68213490@funny-hen.rooster465.autos:443?security=tls&sni=funny-hen.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.197.223.110-0138
    trojan://PI36027154@52.194.192.245:443?security=tls&sni=exciting-grizzly.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.194.192.245-0479
    trojan://CF68213490@sacred-shepherd.rooster465.autos:443?security=tls&sni=sacred-shepherd.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.248.166.163-0244
    trojan://CF68213490@musical-manatee.rooster465.autos:443?security=tls&sni=musical-manatee.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.197.36.228-0179
    trojan://NQ26071394@expert-muskrat.rooster465.autos:443?security=tls&sni=expert-muskrat.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.158.56.149-0169
    trojan://PI36027154@exciting-grizzly.rooster465.autos:443?security=tls&sni=exciting-grizzly.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.194.192.245-0163
    trojan://NQ26071394@gentle-turtle.rooster465.autos:443?security=tls&sni=gentle-turtle.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.114.217.149-0248
    trojan://NQ26071394@alert-wren.rooster465.autos:443?security=tls&sni=alert-wren.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.149.215-0184
    trojan://CF68213490@evolving-mollusk.rooster465.autos:443?security=tls&sni=evolving-mollusk.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.248.6.109-0164
    trojan://NQ26071394@legible-ram.rooster465.autos:443?security=tls&sni=legible-ram.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.183.220.94-0177
    trojan://CF68213490@composed-sheep.rooster465.autos:443?security=tls&sni=composed-sheep.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.65.43.16-0186
    trojan://CF68213490@35.72.9.75:443?security=tls&sni=caring-wallaby.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-35.72.9.75-0140
    trojan://NQ26071394@magical-prawn.rooster465.autos:443?security=tls&sni=magical-prawn.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.176.60.79-0165
    trojan://CF68213490@gentle-honeybee.rooster465.autos:443?security=tls&sni=gentle-honeybee.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.168.247.156-0168
    trojan://CF68213490@careful-penguin.rooster465.autos:443?security=tls&sni=careful-penguin.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.210.229-0139
    trojan://NQ26071394@arriving-koala.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-52.198.192.193-5931
    trojan://CF68213490@informed-stud.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-176.34.18.166-0155
    trojan://CF68213490@13.115.229.63:443?security=tls&sni=alert-redfish.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.115.229.63-0161
    trojan://CF68213490@accurate-frog.rooster465.autos:443?security=tls&sni=accurate-frog.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.65.240.194-0183
    trojan://NQ26071394@grateful-crawdad.rooster465.autos:443?security=tls&sni=grateful-crawdad.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.95.15.6-0142
    trojan://CF68213490@united-molly.rooster465.autos:443?security=tls&sni=united-molly.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.109.243-0141
    trojan://CF68213490@eager-platypus.rooster465.autos:443?security=tls&sni=eager-platypus.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-35.77.85.144-0127
    trojan://NQ26071394@skilled-polliwog.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-57.181.32.234-5862
    trojan://NQ26071394@direct-hawk.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-52.196.147.248-5928
    trojan://NQ26071394@upright-caribou.rooster465.autos:443?security=tls&sni=upright-caribou.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.197.108.120-0157
    trojan://CF68213490@easy-barnacle.rooster465.autos:443?security=tls&sni=easy-barnacle.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.178.0.218-0253
    trojan://NQ26071394@stunning-mastodon.rooster465.autos:443?security=tls&sni=stunning-mastodon.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.231.146.129-0113
    trojan://NQ26071394@elegant-marten.rooster465.autos:443?security=tls&sni=elegant-marten.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.231.110.183-0131
    trojan://CF68213490@funny-hawk.rooster465.autos:443?security=tls&sni=funny-hawk.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.204.233-0137
    trojan://CF68213490@wealthy-gobbler.rooster465.autos:443?security=tls&sni=wealthy-gobbler.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-3.112.189.201-0128
    trojan://NQ26071394@harmless-pegasus.rooster465.autos:443?security=tls&sni=harmless-pegasus.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.214.141-0153
    trojan://CF68213490@eminent-panther.rooster465.autos:443?security=tls&sni=eminent-panther.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.207.117.135-0172
    trojan://HW85960347@sharing-fawn.rooster465.autos:443?security=tls&sni=sharing-fawn.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.179.20.184-0490
    trojan://CF68213490@alert-redfish.rooster465.autos:443?security=tls&sni=alert-redfish.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.115.229.63-0150
    trojan://CF68213490@caring-wallaby.rooster465.autos:443?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-35.72.9.75-0125
    trojan://CF68213490@fair-werewolf.rooster465.autos:443?security=tls&sni=fair-werewolf.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.231.189.62-0117
    trojan://HW85960347@saved-mantis.rooster465.autos:443?security=tls&sni=saved-mantis.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.193.245.102-0495
    trojan://CF68213490@loyal-molly.rooster465.autos:443?security=tls&sni=loyal-molly.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.183.149.237-0120
    trojan://CF68213490@definite-ladybird.rooster465.autos:443?security=tls&sni=definite-ladybird.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-35.77.91.8-0148
    trojan://CF68213490@smiling-fowl.rooster465.autos:443?security=tls&sni=smiling-fowl.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.115.80.163-0158
    trojan://HW85960347@casual-bee.rooster465.autos:443?security=tls&sni=casual-bee.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-13.158.129.149-0403
    trojan://CF68213490@skilled-lioness.rooster465.autos:443?security=tls&sni=skilled-lioness.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.198.124.62-0129
    trojan://CF68213490@adapting-giraffe.rooster465.autos:443?security=tls&sni=adapting-giraffe.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-52.194.255.244-0116
    trojan://JA96378052@bursting-baboon.rooster465.autos:443?security=tls&sni=bursting-baboon.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.179.36.235-0494
    trojan://HW85960347@lucky-primate.rooster465.autos:443?security=tls&sni=lucky-primate.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-18.183.167.54-0492
    trojan://KV63147582@game-firefly.rooster465.autos:443?security=tls#%F0%9F%87%B3%F0%9F%87%B1NL-89.39.70.233-0215
    trojan://CF68213490@communal-sunbird.rooster465.autos:443?security=tls&sni=communal-sunbird.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-43.206.235.148-0118
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@149.22.95.183:443#%F0%9F%87%A8%F0%9F%87%A6CA-149.22.95.183-0104
    trojan://NQ26071394@renewed-phoenix.rooster465.autos:443?security=tls&sni=renewed-phoenix.rooster465.autos#%F0%9F%87%B3%F0%9F%87%B1NL-79.133.126.190-0212
    trojan://CF68213490@nearby-egret.rooster465.autos:443?security=tls&sni=nearby-egret.rooster465.autos#%F0%9F%87%AF%F0%9F%87%B5JP-54.199.102.210-0119
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpoQ0NXT2NJc0s1d3JGejRPWDcwcldm@216.105.168.18:443#%F0%9F%87%BA%F0%9F%87%B8US-216.105.168.18-0190
    trojan://NQ26071394@merry-falcon.rooster465.autos:443?security=tls&sni=merry-falcon.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-13.124.57.203-0198
    trojan://NQ26071394@normal-bull.rooster465.autos:443?security=tls&sni=normal-bull.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-13.124.175.174-0210
    trojan://NQ26071394@gentle-platypus.rooster465.autos:443?security=tls#%F0%9F%87%B0%F0%9F%87%B7KR-52.79.249.115-5967
    trojan://CF68213490@star-bluejay.rooster465.autos:443?security=tls&sni=star-bluejay.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-13.125.159.219-0192
    trojan://CF68213490@charming-puma.rooster465.autos:443?security=tls&sni=charming-puma.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-54.180.1.187-0213
    trojan://NQ26071394@sensible-mongrel.rooster465.autos:443?security=tls&sni=sensible-mongrel.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-52.78.68.191-0209
    trojan://NQ26071394@guided-pelican.rooster465.autos:443?security=tls&sni=guided-pelican.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-43.203.232.180-0203
    trojan://CF68213490@helping-shark.rooster465.autos:443?security=tls&sni=helping-shark.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-3.39.248.52-0204
    trojan://NQ26071394@polished-shrew.rooster465.autos:443?security=tls&sni=polished-shrew.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-43.202.0.42-0199
    trojan://NQ26071394@thorough-foxhound.rooster465.autos:443?security=tls#%F0%9F%87%B0%F0%9F%87%B7KR-43.201.251.27-5856
    trojan://NQ26071394@flexible-titmouse.rooster465.autos:443?security=tls&sni=flexible-titmouse.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-52.78.241.83-0211
    trojan://NQ26071394@modest-amoeba.rooster465.autos:443?security=tls&sni=modest-amoeba.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-43.203.215.162-0207
    trojan://NQ26071394@massive-ocelot.rooster465.autos:443?security=tls&sni=massive-ocelot.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-43.201.253.2-0201
    trojan://CF68213490@smooth-lark.rooster465.autos:443?security=tls#%F0%9F%87%B0%F0%9F%87%B7KR-43.201.46.29-0200
    trojan://NQ26071394@accurate-cat.rooster465.autos:443?security=tls&sni=accurate-cat.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-3.35.176.217-0205
    trojan://CF68213490@climbing-frog.rooster465.autos:443?security=tls&sni=climbing-frog.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-3.35.81.139-0196
    trojan://CF68213490@tolerant-stag.rooster465.autos:443?security=tls&sni=tolerant-stag.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-43.203.209.247-0191
    trojan://CF68213490@central-jawfish.rooster465.autos:443?security=tls#%F0%9F%87%B0%F0%9F%87%B7KR-54.180.233.91-0197
    trojan://CF68213490@gentle-mastiff.rooster465.autos:443?security=tls&sni=gentle-mastiff.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-3.36.60.83-0193
    trojan://NQ26071394@genuine-cougar.rooster465.autos:443?security=tls&sni=genuine-cougar.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-43.202.43.250-0194
    trojan://NQ26071394@living-hagfish.rooster465.autos:443?security=tls&sni=living-hagfish.rooster465.autos#%F0%9F%87%B0%F0%9F%87%B7KR-13.125.78.9-0195
    trojan://XG59623478@concise-buck.rooster465.autos:443?security=tls&sni=concise-buck.rooster465.autos#%F0%9F%87%A6%F0%9F%87%BAAU-82.117.225.216-0218
    trojan://XG59623478@stirring-dane.rooster465.autos:443?security=tls&sni=stirring-dane.rooster465.autos#%F0%9F%87%A6%F0%9F%87%BAAU-82.117.225.56-0222
    trojan://XG59623478@82.117.225.216:443?security=tls&sni=concise-buck.rooster465.autos#%F0%9F%87%A6%F0%9F%87%BAAU-82.117.225.216-0469
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@158.173.20.171:443#%F0%9F%87%B3%F0%9F%87%B1NL-158.173.20.171-0257
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@63.183.207.82:443#%F0%9F%87%A9%F0%9F%87%AADE-63.183.207.82-6018
    trojan://CF68213490@sacred-treefrog.rooster465.autos:443?security=tls&sni=sacred-treefrog.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-52.221.218.103-0246
    trojan://CF68213490@sharp-scorpion.rooster465.autos:443?security=tls&sni=sharp-scorpion.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-18.136.143.231-0245
    trojan://CF68213490@musical-terrier.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-54.255.216.250-0238
    trojan://NQ26071394@allowed-moose.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-54.169.16.108-5981
    trojan://CF68213490@tight-gator.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-54.255.225.60-0251
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@3.75.172.120:443#%F0%9F%87%A9%F0%9F%87%AADE-3.75.172.120-2286
    trojan://CF68213490@learning-wren.rooster465.autos:443?security=tls&sni=learning-wren.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-13.212.190.163-0232
    trojan://NQ26071394@evident-ant.rooster465.autos:443?security=tls&sni=evident-ant.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-13.212.195.78-0223
    trojan://NQ26071394@proper-marlin.rooster465.autos:443?security=tls&sni=proper-marlin.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-54.179.153.60-0234
    trojan://HW85960347@major-cobra.rooster465.autos:443?security=tls&sni=major-cobra.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-54.169.102.170-0489
    trojan://NQ26071394@promoted-rattler.rooster465.autos:443?security=tls&sni=promoted-rattler.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-18.143.94.67-0221
    trojan://CF68213490@active-hippo.rooster465.autos:443?security=tls&sni=active-hippo.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-18.143.179.167-0235
    trojan://CF68213490@summary-lemming.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-52.221.255.155-0242
    trojan://CF68213490@prime-buzzard.rooster465.autos:443?security=tls&sni=prime-buzzard.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-13.212.252.228-0219
    trojan://NQ26071394@helping-newt.rooster465.autos:443?security=tls&sni=helping-newt.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-54.255.178.198-0231
    trojan://CF68213490@gentle-raptor.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-54.169.255.31-0233
    trojan://JA96378052@inspired-goshawk.rooster465.autos:443?security=tls&sni=inspired-goshawk.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-13.212.210.184-0400
    trojan://CF68213490@internal-krill.rooster465.autos:443?security=tls&sni=internal-krill.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-47.131.233.29-0249
    trojan://CF68213490@bright-cicada.rooster465.autos:443?security=tls&sni=bright-cicada.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-47.128.246.104-0236
    trojan://CF68213490@vast-werewolf.rooster465.autos:443?security=tls&sni=vast-werewolf.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-13.229.60.15-0243
    trojan://NQ26071394@topical-shark.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-13.212.141.242-6020
    trojan://CF68213490@modest-bat.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-18.142.251.222-0240
    trojan://CF68213490@relevant-oryx.rooster465.autos:443?security=tls&sni=relevant-oryx.rooster465.autos#%F0%9F%87%B8%F0%9F%87%ACSG-47.129.8.215-0220
    trojan://NQ26071394@amazing-troll.rooster465.autos:443?security=tls#%F0%9F%87%B8%F0%9F%87%ACSG-13.250.26.223-5983

    vmess://ewogICAgImFkZCI6ICJ3d3cuZ292LmhrIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGludXMuY2xvdWRmbGFyZS5xdWVzdCIsCiAgICAiaWQiOiAiMWFiOTFmMTgtNjE2OC00Y2I2LWM5Y2EtMmMzYzcxNThmZTRjIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FyaWVzIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE2LjI0OS4xMzAtMTMwMSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@156.146.38.163:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.163-0799
    vmess://ewogICAgImFkZCI6ICJ4ci0xLmhlcm9rdWFwcC5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ4ci0xLmhlcm9rdWFwcC5jb20iLAogICAgImlkIjogIjE3YWY3NmUxLWE1ZDctNDFhYi1hZTg3LWI0OGYxODUwNzVkMSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8xN2FmNzZlMS1hNWQ3LTQxYWItYWU4Ny1iNDhmMTg1MDc1ZDEtdm1lc3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy01NC4yNDMuMTI5LjIxNS0xOTA1MCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@172.96.192.58:254#%F0%9F%87%BA%F0%9F%87%B8US-172.96.192.58-0463
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@97.64.31.80:247#%F0%9F%87%BA%F0%9F%87%B8US-97.64.31.80-0461
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@144.168.60.70:252#%F0%9F%87%BA%F0%9F%87%B8US-144.168.60.70-15607
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNC4yMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMS50cnVtcDIwMjMubmV0IiwKICAgICJpZCI6ICIxNzZiNTk4Zi00NDViLTQxYWMtOWQyYS00MzBjNWM0ZGYyNmEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNDEuMTAxLjExNC4yMC0wMjk0IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@172.96.192.100:246#%F0%9F%87%BA%F0%9F%87%B8US-172.96.192.100-15615
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJ3d3cuMTcwODAxMDAueHl6IiwKICAgICJpZCI6ICIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xNzM0MTgxNDExMjMiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ny4yMS43Mi40MS01NTE4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDY=@95.169.4.174:254#%F0%9F%87%BA%F0%9F%87%B8US-95.169.4.174-15616
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@104.243.25.95:253#%F0%9F%87%BA%F0%9F%87%B8US-104.243.25.95-0436
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@144.168.58.170:254#%F0%9F%87%BA%F0%9F%87%B8US-144.168.58.170-15618
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@107.182.177.136:256#%F0%9F%87%BA%F0%9F%87%B8US-107.182.177.136-0659
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDY=@93.179.112.70:253#%F0%9F%87%BA%F0%9F%87%B8US-93.179.112.70-15619
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiaWQiOiAiMjU2NmQwMGYtMjE4Yy00OGY3LTlhMzYtMTNkM2Q2ZjFhNzI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMTczNDE4MTQxMTIzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtNjcuMjEuNzIuNDEtOTg3OCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@97.64.122.63:253#%F0%9F%87%BA%F0%9F%87%B8US-97.64.122.63-15606
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjI1NjZkMDBmLTIxOGMtNDhmNy05YTM2LTEzZDNkNmYxYTcyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzE3MzQxODE0MTEyMyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTY3LjIxLjcyLjQxLTQ4OTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJ2dXMyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVzMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy00NS4zMy4xMDUuMjM5LTEwODE3IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJ2dXMzLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVzMy4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy00NS43OS4yMjQuNTMtMTExNyIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJ3d3cuNDg4MTY2MjYueHl6IiwKICAgICJpZCI6ICIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMDgzMDE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ny4yMS43Mi40NC00ODkxIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@198.181.56.163:238#%F0%9F%87%BA%F0%9F%87%B8US-198.181.56.163-15629
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjI1NjZkMDBmLTIxOGMtNDhmNy05YTM2LTEzZDNkNmYxYTcyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzEyMDIwODMwMTQyMiIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTY3LjIxLjcyLjQ0LTEwMzA5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiaWQiOiAiMjU2NmQwMGYtMjE4Yy00OGY3LTlhMzYtMTNkM2Q2ZjFhNzI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMTIwMjA4MzAxNDIyIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtNjcuMjEuNzIuNDQtMTAyODEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.198:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.198-0803
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.79:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.79-0800
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.193:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.193-0998
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.81:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.81-0561
    trojan://e23f408a-012e-4030-8b31-02022031cb50@fhcamd1.gaox.ml:443?allowInsecure=1#%F0%9F%87%BA%F0%9F%87%B8US-129.146.135.157-16738
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.194:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.194-0535
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.195:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.195-0802
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.78:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.78-0533
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.196:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.196-1355
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.80:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.80-0997
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.197:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.197-0562
    vmess://ewogICAgImFkZCI6ICIxMjkuMTU5LjQxLjIzMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMzQxYTkxODItYzQyMy00OTljLWM0NmUtZDE3ODM4YjI5MDM3IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDMyNTg2LAogICAgInBzIjogIvCfh7rwn4e4VVMtMTI5LjE1OS40MS4yMzMtMDIzOSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMjkuMTQ2LjEzMy4xNTciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjgxNzE0Y2VmLTliZGUtNGEwOC1hYTUwLWQ2YmMwMTcyZDc4YiIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiA1MTAwOSwKICAgICJwcyI6ICLwn4e68J+HuFVTLTEyOS4xNDYuMTMzLjE1Ny0wMjc1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTU0LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoNi5zc3ItZnJlZS54eXoiLAogICAgImlkIjogIjVmNjRmYTY1LTdiMTQtNDljNS05NTRkLWFhMTVjNmJmY2FjZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTQuMTUwLTAyNTEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@78.129.253.9:808#%F0%9F%87%AC%F0%9F%87%A7GB-78.129.253.9-15647
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@78.129.253.9:809#%F0%9F%87%AC%F0%9F%87%A7GB-78.129.253.9-1394
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDE=@65.49.204.125:254#%F0%9F%87%BA%F0%9F%87%B8US-65.49.204.125-15627
    vmess://ewogICAgImFkZCI6ICJ2dWsyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVrMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi0xMDkuNzQuMTk0LjIwOC0xMjQ5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:808#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15739
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTU1LjIwMSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMy50cnVtcDIwMjMub3JnIiwKICAgICJpZCI6ICIyOGRhZDY5Yy1jOWQ2LTQ3YzUtYWQwNS1jNjZhZmI4N2NjYmQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjQuMTU1LjIwMS0wMjY2IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxOTguNDEuMjEyLjEwMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZyMS5jZmNkbjEueHl6IiwKICAgICJpZCI6ICJmYjViYmM4Yy1mNmVjLTQ2MjktOGM5ZS0yM2YwMjc4MWEyMGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xOTguNDEuMjEyLjEwMC04NjEwIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:800#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15732
    vmess://ewogICAgImFkZCI6ICJ2ZGUxLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmRlMS4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xNzIuMTA1LjI0NS43OS0wMjk4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJ2ZGUyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmRlMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xMzkuMTQ0LjE3Ni43Ni0xMjgwIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:804#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-14790
    vmess://ewogICAgImFkZCI6ICJzdHJlYW0uYXphZHJhaDIyLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0cmVhbS5hemFkcmFoMjIuY29tIiwKICAgICJpZCI6ICI3NmUxNTFhNy05OTgwLTQwNzctYmQ1Mi0wN2VmNGU5Y2I0OTYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvdXNlciIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh67wn4e3SVItMTg1LjE0My4yMzQuMTIwLTE5NDk5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:805#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15756
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:806#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15744
    vmess://ewogICAgImFkZCI6ICJzdHVkeW5ldy5jbiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0dWR5bmV3LmNuIiwKICAgICJpZCI6ICJiYjg0NzI1YS1mNzI2LTRiY2ItODEzMS00NGRmMTIwOTQwMDUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZGVuZ3FpbmdibyIsCiAgICAicG9ydCI6IDUxMzQwLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTk4LjE0OC4xMjcuNjItOTgxOSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI4NS4xNy41LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIjg1LjE3LjUuMTUwIiwKICAgICJpZCI6ICI0MDcwZmRkZS00M2Q1LTRiM2YtZGJjZi03NzUxYzc3ZTRiZjYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvQWY1NjQ1dHIiLAogICAgInBvcnQiOiAzNjMwNiwKICAgICJwcyI6ICLwn4ez8J+HsU5MLTg1LjE3LjUuMTUwLTExNjE4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICI4NS4xNy41LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNDA3MGZkZGUtNDNkNS00YjNmLWRiY2YtNzc1MWM3N2U0YmY2IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL0FmNTY0NXRyIiwKICAgICJwb3J0IjogMzYzMDYsCiAgICAicHMiOiAi8J+Hs/Cfh7FOTC04NS4xNy41LjE1MC0xMTYxMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:801#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15782
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:807#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0966
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:811#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-2149
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@194.71.126.31:989#%F0%9F%87%B7%F0%9F%87%B8RS-194.71.126.31-0408
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNS4xMjAiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJsZzEuY2ZjZG4zLnh5eiIsCiAgICAiaWQiOiAiMzNhYTU3ZGYtMWM5My00MzE4LTlmY2UtZTg1MDQzN2VlNzgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2Rvbmd0YWl3YW5nLmNvbSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTQxLjEwMS4xMTUuMTIwLTEyMzQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://8b6daf15-8342-482d-b894-1239fd98ce7f@149.56.141.11:443?allowInsecure=1#%F0%9F%87%A8%F0%9F%87%A6CA-149.56.141.11-0319
    ssr://NDUuMTU0LjIxNS4xMzU6MzE1ODA6YXV0aF9hZXMxMjhfc2hhMTphZXMtMjU2LWNmYjp0bHMxLjJfdGlja2V0X2F1dGg6ZW5oUGJXUkUvP29iZnNwYXJhbT1WbTB4TkdFd01VaFNXR2hVVjBkNFYxbHJaRk5XYkd4VlUycFNXRkp0ZUhwWGEyTTFZV3hLZEdWSWNGaGhNVlV4VmtkNFlXTXhXbkZXYkZaWFlsZG9VVmRXVm1GVGJWRjVWR3RXVW1KSGFGbFZha0YzJnJlbWFya3M9OEolMkJIdXZDZmg3aFZVeTAwTlM0eE5UUXVNakUxTGpFek5TMHlNemcxJnByb3RvcGFyYW09TWpJMk5qTTZVWEZNYjJGWg==
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMTY5ODkiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://8b6daf15-8342-482d-b894-1239fd98ce7f@cat1.sshocean.net:443?allowInsecure=1#%F0%9F%87%A8%F0%9F%87%A6CA-149.56.141.11-0241
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo5N09uREVaWUdqYTQ=@178.18.244.2:443#%F0%9F%87%A9%F0%9F%87%AADE-178.18.244.2-0756
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpzaUY5OHhCTDJ2MWk=@135.181.114.242:8478#%F0%9F%87%AB%F0%9F%87%AEFI-135.181.114.242-0798
    ss://YWVzLTI1Ni1jZmI6R2VyZWdldFI4Y3ZRSHpZcg==@213.183.53.221:9030#%F0%9F%87%B7%F0%9F%87%BARU-213.183.53.221-15695
    ss://YWVzLTI1Ni1jZmI6ZjhucEtnTnpka3NzMnl0bg==@213.183.53.221:9088#%F0%9F%87%B7%F0%9F%87%BARU-213.183.53.221-15694
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTopMU4xRTZ2MFNVX3JHVHBn@38.64.138.53:1035#%F0%9F%87%BA%F0%9F%87%B8US-38.64.138.53-0573
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.47:805#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.47-0761
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:812#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15779
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpXYWN3ZXRDaWY=@217.12.223.190:444#%F0%9F%87%BA%F0%9F%87%A6UA-217.12.223.190-0790
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:808#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-13651
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@5.188.0.151:800#%F0%9F%87%BA%F0%9F%87%B8US-5.188.0.151-15704
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@ak1466.free.www.outline.network:811#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-7643
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:809#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0566
    ssr://anAtYW00OC02LmVxbm9kZS5uZXQ6ODA4MTpvcmlnaW46YWVzLTI1Ni1jZmI6dGxzMS4yX3RpY2tldF9hdXRoOlpVRnZhMkpoUkU0Mi8/b2Jmc3BhcmFtPSZyZW1hcmtzPThKJTJCSHIlMkZDZmg3VktVQzAxTkM0Mk5DNDFOeTR6TkMwd05UYzQmcHJvdG9wYXJhbT0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:805#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15687
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiNTEuODkuNDIuMTU0IiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMTEzNTciLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNS4yIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZnIxLmNmY2RuMS54eXoiLAogICAgImlkIjogImZiNWJiYzhjLWY2ZWMtNDYyOS04YzllLTIzZjAyNzgxYTIwZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE0MS4xMDEuMTE1LjItMDI0NCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNTAuMjMwLjE5OS4xNzciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjZiNzQ1Y2FmLWU3ZjYtNDlmMS05YjYzLWU1YzQxNjMwM2JhYyIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAyMTY5NiwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1MC4yMzAuMTk5LjE3Ny0wMjM3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNDQuMjQuODguMTAxIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJmNTQyNWNjZi0zOTQ2LTRmYjQtZWIyNC01MzkzZDc4YTM5MmYiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTY4MzMsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNDQuMjQuODguMTAxLTA0NzYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.143:802#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.143-15751
    vmess://ewogICAgImFkZCI6ICIxMzguMi4xNS4yMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTk4MTUxZTUtMGJjNS00Mzc3LWUzOTAtYzQxYmIyNmZkZDBjIiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDQ2MzcwLAogICAgInBzIjogIvCfh6/wn4e1SlAtMTM4LjIuMTUuMjMtMDI5MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJ2bTEyLmxlaWZlbmdrZWppLmxpdmUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ2bTEyLmxlaWZlbmdrZWppLmxpdmUiLAogICAgImlkIjogIjc1MmE5NDA0LWM3MjktNDg1ZS04ZWE1LWFjYjNmNGZjODE4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAxMTExMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTQzLjIwMS4zOC4xOTMtMTI5OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJ2bTUubGVpZmVuZ2tlamkubGl2ZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInZtNS5sZWlmZW5na2VqaS5saXZlIiwKICAgICJpZCI6ICI3NTJhOTQwNC1jNzI5LTQ4NWUtOGVhNS1hY2IzZjRmYzgxODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTExMTEsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xMy4yMDkuNC4yMTEtMDIyOCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://752a9404-c729-485e-8ea5-acb3f4fc8180@hg5.leifengkeji.live:48903?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-43.200.4.201-11721
    vmess://ewogICAgImFkZCI6ICIxNTIuNzAuMjQxLjE4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJlY2QyNzRjMC0xNzVkLTQ1ZjctODI3Ni1hM2RhOTM3ODY2MzIiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMjY2NzYsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNTIuNzAuMjQxLjE4LTAzMjgiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxOTIuNzQuMjQyLjE4MiIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjQxODA0OGFmLWEyOTMtNGI5OS05YjBjLTk4Y2EzNTgwZGQyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzE3MDQxOTExMTAyMSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTE5Mi43NC4yNDIuMTgyLTE2NjgzIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICJ3d3cuMzIzMzgwNzUueHl6Igp9
    vmess://ewogICAgImFkZCI6ICJ2bTgubGVpZmVuZ2tlamkubGl2ZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInZtOC5sZWlmZW5na2VqaS5saXZlIiwKICAgICJpZCI6ICI3NTJhOTQwNC1jNzI5LTQ4NWUtOGVhNS1hY2IzZjRmYzgxODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTExMTEsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNS4xNjQuMTYzLjE0LTExODg0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://752a9404-c729-485e-8ea5-acb3f4fc8180@hg17.leifengkeji.live:33387?allowInsecure=1&sni=hg17.leifengkeji.live#%F0%9F%87%B0%F0%9F%87%B7KR-15.164.103.48-0255
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:803#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0571
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.143:805#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.143-15766
    vmess://ewogICAgImFkZCI6ICIxNDYuNTYuMTU1LjcwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJmOTc3MWMxOS1jOTFjLTQxYjUtOTA2NC04NzY4YjUxY2VjNmQiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTgwNTAsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNDYuNTYuMTU1LjcwLTAzMjUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:801#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15760
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:803#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15754
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:802#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0537
    trojan://0Y9gOHSdRt@150.230.249.42:443?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-150.230.249.42-0291
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:805#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-0771
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:800#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15677
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:806#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0553
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiWW91VHViZS1hd2Vpa2VqaSIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtMTU1NDUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:800#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0543
    vmess://ewogICAgImFkZCI6ICI4LjIwOS4yMTguMTk1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGluZG8uY25hYmMuZXUub3JnIiwKICAgICJpZCI6ICJmNmQ3YjA3Mi1kZTAwLTQ1ZGMtOWUyNC00OWY4Y2Y0MzUzMGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlub2QiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC04LjIwOS4yMTguMTk1LTAzMjYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJ2bTE1LmxlaWZlbmdrZWppLmxpdmUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ2bTE1LmxlaWZlbmdrZWppLmxpdmUiLAogICAgImlkIjogIjc1MmE5NDA0LWM3MjktNDg1ZS04ZWE1LWFjYjNmNGZjODE4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAxMTExMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTU0LjE4MC4xMDEuNi0wMjkzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJhZWFkanBhZXMwMS54bi0tejRxNDhsY3ZwLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNob3V0aW5ndG91dGlhbzMuMTAwMTAuY29tIiwKICAgICJpZCI6ICIzZTgyMGViMC0zZjA2LTQzMzctYTRmYy0wYzNjN2MwZDNiNGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaW1hZ2VzIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC0xNzIuMTA0Ljc5Ljk2LTE2MTA3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTUyLjY3LjIxOC4zOCIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtMDIyNCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMjkuMTU0LjU3LjEzNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiY2FiYmRmNWQtM2NjYS00NjA1LWJhMWMtYzg5YTdkNWI0YzA3IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDI2MjgyLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTI5LjE1NC41Ny4xMzQtMDMyMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp2QXBZaUFnaHplc0g=@217.70.188.60:855#%F0%9F%87%AB%F0%9F%87%B7FR-217.70.188.60-15709
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMjM3OSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJtNC40MDAxMDAxMC54eXoiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjU3NWU0ZDkyLTEwNTYtNDRjMi04Y2FjLTc1ZWYxYzg1OWFkNSIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAzNzEyMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE0Ni41Ni4xMzMuMTA5LTAyODUiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:800#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10336
    vmess://ewogICAgImFkZCI6ICJ3d3cuYXB1bG5pb24uY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAid3d3LmFwdWxuaW9uLmNvbSIsCiAgICAiaWQiOiAiN2I4YzM3MGQtODYxMC00OTg4LWIwYTctY2RlNzRhYTA3MTNiIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLzU4YTUzNDJmN2EvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTMyLjIyNi4xNzMuMTE4LTAzMzEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNTIuNzAuMjM1LjIwNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNzBkOTUzMDgtMmE2MS00ZjkzLWYxMzktOTEwM2QwNTg3ZmQ5IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDM1NDEyLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTUyLjcwLjIzNS4yMDctMDI3MSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZG0udG91dGlhby5jb20iLAogICAgImlkIjogIjY4ZGY0ODM4LTQ2ZDAtNGI1Yi1jM2YwLWE0MGVjNzA2MzI0NSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4e48J+HrFNHLTE4LjE0My4xMjMuMzUtMTU3MzMiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:804#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0555
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI2OGRmNDgzOC00NmQwLTRiNWItYzNmMC1hNDBlYzcwNjMyNDUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xOC4xNDMuMTIzLjM1LTAzMzciLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://bb5b1337-fa9e-4e00-b8c6-1110e626171d@159.223.89.239:443?allowInsecure=1#%F0%9F%87%B8%F0%9F%87%ACSG-159.223.89.239-0240
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTguMTQzLjEyMy4zNSIsCiAgICAiaWQiOiAiNjhkZjQ4MzgtNDZkMC00YjViLWMzZjAtYTQwZWM3MDYzMjQ1IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh7jwn4esU0ctMTguMTQzLjEyMy4zNS0xNTcyMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://bb5b1337-fa9e-4e00-b8c6-1110e626171d@sg-01.tiktokcdn.top:443?allowInsecure=1#%F0%9F%87%B8%F0%9F%87%ACSG-159.223.89.239-0282
    vmess://ewogICAgImFkZCI6ICIxMzguMi40NC4yMTEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjU5M2I4NTI1LTBjNDgtNGIwZi1kOWFmLTJkNzNhOTE0ODk3MyIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAyMDA4MSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTEzOC4yLjQ0LjIxMS0wMjYzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3LjYwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhYzhlMjZmZS04MTUwLTRiNjAtYWU2NC04MmZjNzdlYmEyY2YiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTA2OSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNjAtMTM5OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNjcuMTcyLjY0LjExIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI3NmEyNzZhMi0wZmMzLTRiZmItY2IwMC02Y2QyYTQzMDk2NzciLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTAwODYsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xNjcuMTcyLjY0LjExLTAyMzQiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3LjYwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhYzhlMjZmZS04MTUwLTRiNjAtYWU2NC04MmZjNzdlYmEyY2YiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTA2OSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNjAtMDMyMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJzZzIwMi5oa2FhMC50ayIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNnMjAyLmhrYWEwLnRrIiwKICAgICJpZCI6ICJiZGY3OThmNC1hOTkwLTQ3NDMtZTliMi05Yzc4YmE1OGZiMDQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaGthYTAiLAogICAgInBvcnQiOiAxMDE4LAogICAgInBzIjogIvCfh7jwn4esU0ctMTcyLjEwNC4xNjMuMjAyLTE3MDg3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICJzZzIwMi5oa2FhMC50ayIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:809#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15659
    ss://YWVzLTI1Ni1jZmI6dkRTOUcycA==@185.4.65.6:21247#%F0%9F%87%B7%F0%9F%87%BARU-185.4.65.6-15714
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:803#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15657
    trojan://cb43b7c2-b744-41c5-bcc2-fd7467b332cf@jgwxn3.gaox.ml:443?allowInsecure=1#%F0%9F%87%A6%F0%9F%87%BAAU-140.238.205.173-14885
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:805#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0538
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:809#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15778
    trojan://c19d1432-8b3e-4818-8837-3d160cf65908@138.2.45.243:443?allowInsecure=1#%F0%9F%87%AF%F0%9F%87%B5JP-138.2.45.243-19249
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:809#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10334
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:804#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15656
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:802#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15689
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:805#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15679
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTUzLjEwMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMi50cnVtcDIwMjMudXMiLAogICAgImlkIjogImJlZDNkODc2LTJkMjYtNGQ0ZC1iNzg5LTMwNjM0MzhlZTc3NCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTMuMTAyLTEwNTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:809#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15688
    vmess://ewogICAgImFkZCI6ICIxNi4xNjIuNTUuMTMwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTYuMTYyLjU1LjEzMCIsCiAgICAiaWQiOiAiMTliOTVhMGUtZmZjZi0zMmVkLTg2NTYtNTJhZTEwMmE4YWQ4IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL255IiwKICAgICJwb3J0IjogNDQzMDAsCiAgICAicHMiOiAi8J+HrfCfh7BISy0xNi4xNjIuNTUuMTMwLTEyMzcxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:812#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0545
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:811#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15770
    vmess://ewogICAgImFkZCI6ICIxMzkuOTkuOTEuOTUiLAogICAgImFpZCI6IDMyLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJjMDE1NjQ1MS00ZWZiLTQ1ZTItODRmYy04ZDMxNWM0NjUwZGIiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7jwn4esU0ctMTM5Ljk5LjkxLjk1LTAyMzIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:810#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10335
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:812#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15693
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:808#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15691
    ss://YWVzLTI1Ni1jZmI6ZjYzZ2c4RXJ1RG5Vcm16NA==@213.183.59.214:9010#%F0%9F%87%B3%F0%9F%87%B1NL-213.183.59.214-17493
    vmess://ewogICAgImFkZCI6ICJzZy1vdmgxLnYyLXJheS5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJzZy1vdmgxLnYyLXJheS5jb20iLAogICAgImlkIjogImE5NDgxNjAwLWVmMzYtNDAyYS1hMGU1LTU1NDdiZmQ3Yjg3YyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9mYXN0c3NoL2ZnaGhoLzYzNDE5N2M0Y2RmODEvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7jwn4esU0ctNTEuNzkuMTY0LjE0Ni0yNzc4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://e05c749b-7c6b-41b8-9c71-9dcf685edf4a@152.67.162.166:443?allowInsecure=1&sni=content-provider22.cdn-delivery.akamaicd.com#%F0%9F%87%AE%F0%9F%87%B3IN-152.67.162.166-4645
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpxWUF0ODVTRkdWNTY=@185.77.217.217:443#%F0%9F%87%AB%F0%9F%87%AEFI-185.77.217.217-0797
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:811#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-10525
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:804#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15768
    vmess://ewogICAgImFkZCI6ICJmdWxsYWNjZXNzdG9rb3JlYW5uZXRzdWJub2RlMS5henVyZXdlYnNpdGVzLm5ldCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZ1bGxhY2Nlc3N0b2tvcmVhbm5ldHN1Ym5vZGUxLmF6dXJld2Vic2l0ZXMubmV0IiwKICAgICJpZCI6ICIyNzRmMTFjNi1mNjliLTQwYjktODk2Ni1mMzllMDZlOTdiZTciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvd3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HsPCfh7dLUi01Mi4yMzEuMjAwLjE3OS01MDI5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:809#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-10984
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:810#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-0772
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:804#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15753
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:803#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15777
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.47:800#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.47-15661
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:800#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-21268
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:805#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15767
    vmess://ewogICAgImFkZCI6ICIxNjguMTM4LjIwNy42NiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTA1Zjk5YjEtZTdiYS00NWUwLWFlNGQtYjBmZmRmMGFkMjQ1IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDIxMzY1LAogICAgInBzIjogIvCfh6/wn4e1SlAtMTY4LjEzOC4yMDcuNjYtMDI2NyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTopMU4xRTZ2MFNVX3JHVHBn@79.133.109.56:1036#%F0%9F%87%BA%F0%9F%87%B8US-79.133.109.56-15762
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:809#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15775
    vmess://ewogICAgImFkZCI6ICJ3d3cuZ292LmhrIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidm4uY2xvdWRmbGFyZS5xdWVzdCIsCiAgICAiaWQiOiAiZGM4YjY0ZGItZWI2ZC00YmRmLTk4YjItMzE2MTUzMTliZWE4IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FyaWVzIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE2LjI0OS4xMzAtMTI5NSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxODUuMjI1LjY5LjEzNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiM2MzYmZkNzUtZGMzMC00ZTc2LTg5NDAtNDdlMTEzN2UyMWY5IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDQ1MDgxLAogICAgInBzIjogIvCfh63wn4e6SFUtMTg1LjIyNS42OS4xMzQtMDIyMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:810#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15761
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:801#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15719
    vmess://ewogICAgImFkZCI6ICJzZzExOC5oa2FhMC50ayIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNnMTE4LmhrYWEwLnRrIiwKICAgICJpZCI6ICI2NTJmNDI2My1iZDg2LTRiZjYtOWY3ZS1kMjVlNzUxNmZiNzIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaGthYTAiLAogICAgInBvcnQiOiAxMzY5MSwKICAgICJwcyI6ICLwn4e48J+HrFNHLTE3Mi4xMDQuMTYzLjExOC0wMjQ4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:804#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10332
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:800#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15681
    vmess://ewogICAgImFkZCI6ICJ2c2cxLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiJTdCJTIySG9zdCUyMjolMjJ2c2cxLjBiYWQuY29tJTIyJTdEIiwKICAgICJpZCI6ICI5MjcwOTRkMy1kNjc4LTQ3NjMtODU5MS1lMjQwZDBiY2FlODciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvY2hhdCIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e48J+HrFNHLTE3MC4xODcuMTk2LjEyOC0xNTk4MSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI4OS4yMDguMTA1LjYzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICIyRjA5NDg0NS1FMkJELUVCRjctREVCNy05OTU5OTI0MzZGQUYiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMjM0NTMsCiAgICAicHMiOiAi8J+Hs/Cfh7FOTC04OS4yMDguMTA1LjYzLTAzMDYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:802#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15692
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:812#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-0765
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:807#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20430
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:812#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15660
    trojan://3f087c04-44e6-4c96-a917-ca974de1212b@kr1.api-aws.com:443?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-146.56.176.239-15564
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:803#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10337
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTUzLjEwMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMi50cnVtcDIwMjMudXMiLAogICAgImlkIjogImJlZDNkODc2LTJkMjYtNGQ0ZC1iNzg5LTMwNjM0MzhlZTc3NCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTMuMTAyLTAyNTIiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:805#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20428
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:801#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-2879
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:810#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20415
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:808#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20437
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:802#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20423
    vmess://ewogICAgImFkZCI6ICJ1bnVzMDEuYWpka2phbGpkai54eXoiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ1bnVzMDEuYWpka2phbGpkai54eXoiLAogICAgImlkIjogIjk1ZTlmZGExLWRjNDgtM2JiZC04YTE1LWU2NTI4ODgyZWEzYiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi82IiwKICAgICJwb3J0IjogMTA4MiwKICAgICJwcyI6ICLwn4e68J+HuFVTLTM4LjU0Ljk1LjE3OC01MjQxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:800#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20418
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:800#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-4617
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.159.30.61:808#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.30.61-0082
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@193.176.86.190:806#%F0%9F%87%A9%F0%9F%87%AADE-193.176.86.190-0969
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:801#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-0967
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:806#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-0763
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:801#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15655
    vmess://ewogICAgImFkZCI6ICIyMTMuMjI2LjcxLjEyNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMkYwOTQ4NDUtRTJCRC1FQkY3LURFQjctOTk1OTkyNDM2RkFGIiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDIzNDUzLAogICAgInBzIjogIvCfh6nwn4eqREUtMjEzLjIyNi43MS4xMjctNzkyNCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:807#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7529
    vmess://ewogICAgImFkZCI6ICJzZy5wcnByLmxpbmsiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJzZy5wcnByLmxpbmsiLAogICAgImlkIjogImNlYTQyMTYxLWJkZGMtNDIzMC1hOWI5LWU0MzE4Nzk2N2ZmYSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9UZWxlZ3JhbS9TaGFyZUNlbnRyZVByby9ta25uaXgiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS4zNS4yMTEtMTI1OCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:809#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7524
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:810#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-2099
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:804#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7527
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:808#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7521
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.159.30.61:809#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.30.61-1423
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:802#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7526
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpVbHRyQHIwMHRfMjAxNw==@138.68.248.130:811#%F0%9F%87%BA%F0%9F%87%B8US-138.68.248.130-0556

</details>

-   you can import these 200 tested nodes using their subscription link into different clients. refer to `Instructions & Usage` section

### all nodes
merge nodes w/o dup: `5296`
merge nodes w/o dup: `7004`

-   [Node link Mixed (V2ray)](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/sub_merge.txt)
-   [Node link Yaml (Clash)](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/sub_merge_yaml.yml)

#### all nodes separated by protoctol

-   [VMESS](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/splitted/vmess.txt)
-   [TROJAN](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/splitted/trojan.txt)
-   [SSR](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/splitted/ssr.txt)
-   [SHADOWSOCKS](https://raw.githubusercontent.com/SSgumS/V2RayAggregator/master/sub/splitted/ss.txt)

#### provider config for clash 🐈‍⬛

> Configs with the "others" tag will proxy domestic services.

-   [Clash Meta For Iran](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta.yml) (Recommended)
-   [Clash Meta For China](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta-cn.yml) (Recommended)
-   [Clash Meta For Others](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta-others.yml) (Recommended)

-   [Clash For Iran](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider.yml)
-   [Clash For China](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-cn.yml)
-   [Clash For Others](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-others.yml)

### node sources
- [pojiezhiyuanjun/freev2](https://github.com/pojiezhiyuanjun/freev2), number of nodes: `63`
- [SSgumS/V2RayAggregator](https://github.com/SSgumS/V2RayAggregator), number of nodes: `200`
- [iwxf/free-v2ray](https://github.com/iwxf/free-v2ray), number of nodes: `39`
- [DoveBoy/Vmess-Actions](https://github.com/ldir92664/Vmess-Actions), number of nodes: `105`
- [gooooooooooooogle/Clash-Config](https://github.com/gooooooooooooogle/Clash-Config), number of nodes: `1`
- [ermaozi/get_subscribe](https://github.com/ermaozi/get_subscribe), number of nodes: `16`
- [wrfree/free](https://github.com/wrfree/free), number of nodes: `51`
- [anaer/Sub](https://github.com/anaer/Sub), number of nodes: `1570`
- [Pawdroid/Free-servers](https://github.com/Pawdroid/Free-servers), number of nodes: `7`
- [misersun/config003-002](https://github.com/misersun/config003), number of nodes: `217`
- [mfuu/v2ray](https://github.com/mfuu/v2ray), number of nodes: `198`
- [freefq/free](https://github.com/freefq/free), number of nodes: `14`
- [xiyaowong/freeFQ](https://github.com/xiyaowong/freeFQ), number of nodes: `156`
- [YasserDivaR/pr0xy](https://github.com/YasserDivaR/pr0xy), number of nodes: `621`
- [peasoft/NoMoreWalls](https://github.com/peasoft/NoMoreWalls), number of nodes: `38`
- [mahdibland/get_v2](https://github.com/mahdibland/get_v2), number of nodes: `2373`
- [jikelonglie/meskell](https://github.com/jikelonglie/meskell), number of nodes: `9`
- [freebaipiao/freebaipiao](https://github.com/freebaipiao/freebaipiao), number of nodes: `6`
- [MOnday9907/v2ray](https://github.com/MOnday9907/v2ray), number of nodes: `8`
- [adminaliang/v2ray](https://github.com/adminaliang/v2ray), number of nodes: `16`
- [Jia-Pingwa/free-v2ray-merge](https://github.com/Jia-Pingwa/free-v2ray-merge), number of nodes: `327`
- [Lewis-1217/FreeNodes](https://github.com/Lewis-1217/FreeNodes), number of nodes: `39`
- [jiang.netlify.app](https://jiang.netlify.app), number of nodes: `20`
- [learnhard-cn/free_proxy_ss](https://github.com/learnhard-cn/free_proxy_ss), number of nodes: `116`
- [SnapdragonLee/SystemProxy](https://github.com/SnapdragonLee/SystemProxy), number of nodes: `357`
- [hermanb001/ProxyTest](https://github.com/hermanb001/ProxyTest), number of nodes: `1743`
- [mahdibland/vpn.fail](https://github.com/mahdibland/get_v2), number of nodes: `1000`
- [LonUp/NodeList](https://github.com/LonUp/NodeList), number of nodes: `1451`

-   [pojiezhiyuanjun/freev2](https://github.com/pojiezhiyuanjun/freev2), number of nodes: `162`
-   [Nodefree.org](https://github.com/Fukki-Z/nodefree), number of nodes: `39`
-   [mianfeifq/share](https://github.com/mianfeifq/share), number of nodes: `103`
-   [FiFier/v2rayShare](https://github.com/FiFier/v2rayShare), number of nodes: `39`
-   [huanongkejizhijia/clashnode](https://github.com/huanongkejizhijia/clashnode), number of nodes: `44`
-   [RenaLio/Mux2sub](https://github.com/RenaLio/Mux2sub), number of nodes: `134`
-   [colatiger/v2ray-nodes](https://github.com/colatiger/v2ray-nodes), number of nodes: `121`
-   [oslook/clash-freenode](https://github.com/oslook/clash-freenode), number of nodes: `44`
-   [ssrsub/ssr](https://github.com/ssrsub/ssr), number of nodes: `231`
-   [SSgumS/V2RayAggregator](https://github.com/SSgumS/V2RayAggregator), number of nodes: `200`
-   [iwxf/free-v2ray](https://github.com/iwxf/free-v2ray), number of nodes: `39`
-   [DoveBoy/Vmess-Actions](https://github.com/ldir92664/Vmess-Actions), number of nodes: `105`
-   [gooooooooooooogle/Clash-Config](https://github.com/gooooooooooooogle/Clash-Config), number of nodes: `1`
-   [Jsnzkpg/Jsnzkpg](https://github.com/Jsnzkpg/Jsnzkpg), number of nodes: `18`
-   [ermaozi/get_subscribe](https://github.com/ermaozi/get_subscribe), number of nodes: `39`
-   [wrfree/free](https://github.com/wrfree/free), number of nodes: `51`
-   [anaer/Sub](https://github.com/anaer/Sub), number of nodes: `398`
-   [aiboboxx/v2rayfree](https://github.com/aiboboxx/v2rayfree), number of nodes: `43`
-   [Pawdroid/Free-servers](https://github.com/Pawdroid/Free-servers), number of nodes: `17`
-   [Rokate/Proxy-Sub](https://github.com/Rokate/Proxy-Sub), number of nodes: `97`
-   [misersun/config003-002](https://github.com/misersun/config003), number of nodes: `217`
-   [clash.221207.xyz/pubclashyaml](https://clash.221207.xyz/pubclashyaml), number of nodes: `787`
-   [tbbatbb/Proxy](https://github.com/tbbatbb/Proxy), number of nodes: `586`
-   [mfuu/v2ray](https://github.com/mfuu/v2ray), number of nodes: `436`
-   [openRunner/clash-freenode](https://github.com/openRunner/clash-freenode), number of nodes: `44`
-   [freefq/free](https://github.com/freefq/free), number of nodes: `30`
-   [xiyaowong/freeFQ](https://github.com/xiyaowong/freeFQ), number of nodes: `156`
-   [yaney01/Yaney01](https://github.com/yaney01/Yaney01), number of nodes: `654`
-   [YasserDivaR/pr0xy](https://github.com/YasserDivaR/pr0xy), number of nodes: `1245`
-   [peasoft/NoMoreWalls](https://github.com/peasoft/NoMoreWalls), number of nodes: `425`
-   [mahdibland/get_v2](https://github.com/mahdibland/get_v2), number of nodes: `2353`
-   [vveg26/get_proxy](https://github.com/vveg26/get_proxy), number of nodes: `629`
-   [free.jingfu.cf/clash](https://free.jingfu.cf/clash), number of nodes: `97`
-   [AzadNetCH/Clash](https://github.com/AzadNetCH/Clash), number of nodes: `6582`
-   [proxy.yugogo.xyz/clash](https://proxy.yugogo.xyz/clash), number of nodes: `319`
-   [jikelonglie/meskell](https://github.com/jikelonglie/meskell), number of nodes: `9`
-   [freebaipiao/freebaipiao](https://github.com/freebaipiao/freebaipiao), number of nodes: `6`
-   [huwo1/proxy_nodes](https://bitbucket.org/huwo1/proxy_nodes/src/main), number of nodes: `183`
-   [lisylva-lee/v2dyku](https://github.com/lisylva-lee/v2dyku), number of nodes: `14`
-   [budamu/clashconfig](https://github.com/budamu/clashconfig), number of nodes: `142`
-   [MOnday9907/v2ray](https://github.com/MOnday9907/v2ray), number of nodes: `8`
-   [adminaliang/v2ray](https://github.com/adminaliang/v2ray), number of nodes: `16`
-   [Jia-Pingwa/free-v2ray-merge](https://github.com/Jia-Pingwa/free-v2ray-merge), number of nodes: `327`
-   [Lewis-1217/FreeNodes](https://github.com/Lewis-1217/FreeNodes), number of nodes: `63`
-   [youlianboshi.netlify.app](https://youlianboshi.netlify.app), number of nodes: `7`
-   [jiang.netlify.app](https://jiang.netlify.app), number of nodes: `16`
-   [learnhard-cn/free_proxy_ss](https://github.com/learnhard-cn/free_proxy_ss), number of nodes: `250`
-   [SnapdragonLee/SystemProxy](https://github.com/SnapdragonLee/SystemProxy), number of nodes: `244`
-   [sub.pmsub.me/base64](https://sub.pmsub.me/base64), number of nodes: `606`
-   [hermanb001/ProxyTest](https://github.com/hermanb001/ProxyTest), number of nodes: `1743`
-   [LonUp/NodeList](https://github.com/LonUp/NodeList), number of nodes: `1451`

## Softwares

### Best Clients For Each OS

|   OS    |               Best Client               | Alternatives |
| :-----: | :-------------------------------------: | :----------: |
|   IOS   |        Quantumult - Shadowrocket        | NapsternetV  |
| Android | Surfboard - Clash For Android - Matsuri |   V2rayNg    |
| Windows |  Clash For Windows - V2rayN - Nekoray   |    Qv2ray    |
|  Linux  |            Clash For Windows            |    Qv2ray    |
|  MacOS  |            Clash For Windows            |    Qv2ray    |

### Desktop Clients

|                              MacOS                               |                              Linux                               |                                       Windows                                       | Brief description                                                                                                                                                        |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :---------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW(Clash For Windows)](https://github.com/Fndroid/clash_for_windows_pkg/releases) | SS, SSR, Trojan, Vmess, VLESS protocol support, strong policy offload capability.                                                                                        |
|       [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)        |       [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)        |                 [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)                 | SS, SSR, Trojan, Vmess, VLESS, Trojan-Go protocol support (relevant plugins need to be installed).                                                                       |
|                                ×                                 |                                ×                                 |                 [V2rayN](https://github.com/2dust/v2rayN/releases)                  | SS, Trojan, Vmess, VLESS protocol support, with speed measurement, delay measurement function, support subscription, QR code, clipboard import and manual configuration. |
|                                ×                                 |                                ×                                 |               [WinXray](https://github.com/TheMRLL/winxray/releases)                | SS, SSR, Trojan, Vmess, VLESS protocol support, support automatic connection to the fastest node.                                                                        |
|                                ×                                 |                                ×                                 | [Shadowsocks-windows](https://github.com/shadowsocks/shadowsocks-windows/releases)  | SS protocol support, SS dedicated client.                                                                                                                                |
|                                ×                                 |                                ×                                 |  [ShadowsocksR-windows](https://github.com/HMBSbige/ShadowsocksR-Windows/releases)  | SSR protocol support, SSR dedicated client.                                                                                                                              |
|                  [Surge](https://nssurge.com/)                   |                                ×                                 |                                          ×                                          | SS, Trojan, Vmess protocol support, well-known network debugging tools, powerful strategy offloading ability, need to pay.                                               |
|     [ClashX](https://github.com/yichengchen/clashX/releases)     |                                ×                                 |                                          ×                                          | SS, SSR, Trojan, Vmess protocol support, occupy less resources.                                                                                                          |
|        [V2rayU](https://github.com/yanue/V2rayU/releases)        |                                ×                                 |                                          ×                                          | SS, Trojan, Vmess protocol support, support subscription, QR code, clipboard import, manual configuration, QR code sharing, similar to V2RayN.                           |
|       [V2rayA](https://github.com/v2rayA/v2rayA/releases/)       |       [V2rayA](https://github.com/v2rayA/v2rayA/releases/)       |                [V2rayA](https://github.com/v2rayA/v2rayA/releases/)                 | V2Ray, Xray, SS, SSR, Trojan support, subscription and manual config.                                                                                                    |

### Mobile Clients

|                               iOS/iPadOS                                |                                      Android                                       | Brief description                                                                                                                                                                                                                                                 |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)  |  [Shadowrocket](https://play.google.com/store/apps/details?id=com.v2cross.proxy)   | SS, SSR, Trojan, Vmess, VLESS protocol support, the iOS side needs to be purchased in the non-country App Store, the US price is $2.99; the Android side is not the same author as the iOS side, does not support the SSR protocol, free and built-in free nodes. |
|                      [Surge](https://nssurge.com/)                      |                                         ×                                          | SS, Trojan, Vmess protocol support, well-known network debugging tools on the iOS side, chargeable.                                                                                                                                                               |
| [Quantumult X](https://apps.apple.com/us/app/quantumult-x/id1443988620) |                                         ×                                          |                                                                                                                                                                                                                                                                   |
| [Potatso Lite](https://apps.apple.com/us/app/potatso-lite/id1239860606) |                                         ×                                          | SS, SSR protocol support, need to be purchased in the non-country AppStore, free.                                                                                                                                                                                 |
|                                    ×                                    |    [Surfboard](https://play.google.com/store/apps/details?id=com.getsurfboard)     | SS, SSR, Vmess Protocol support, Android network debugging software, compatible with Surge 2 configuration.                                                                                                                                                       |
|                                    ×                                    |    [CFA(Clash For Android)](https://github.com/Kr328/ClashForAndroid/releases)     | SS, SSR, Trojan, Vmess Protocol support.                                                                                                                                                                                                                          |
|                                    ×                                    |             [SagerNet](https://github.com/SagerNet/SagerNet/releases)              | SS, SSR, Trojan, Vmess, VLESS Protocol support.                                                                                                                                                                                                                   |
|                                    ×                                    | [Shadowsocks-android](https://github.com/shadowsocks/shadowsocks-android/releases) | SS protocol support, Android-specific SS client.                                                                                                                                                                                                                  |
|                                    ×                                    | [ShadowsocksR-android](https://github.com/HMBSbige/ShadowsocksR-Android/releases)  | SSR protocol support, Android-specific SSR client.                                                                                                                                                                                                                |
|                                    ×                                    |                [V2rayNG](https://github.com/2dust/v2rayNG/releases)                | SS, Trojan, Vmess, VLESS protocol support, v2ray kernel.                                                                                                                                                                                                          |

### Credit:

-   [alanbobs999](https://github.com/alanbobs999)
-   [PersianBlocker](https://github.com/MasterKia/PersianBlocker)
-   [iran-hosted-domains](https://github.com/bootmortis/iran-hosted-domains)

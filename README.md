# eJPT-Skill-Check-Lab-FootPrinting-Scanning
FootPrinting &amp; Scanning - eJPT Skill Check Lab (Capture The Flag)

**Activity Type:** Passive & Active Footprinting + Scanning  
**Target:** `http://target.ine.local`  
**Environment:** eJPT Practice Lab (Capture The Flag → INE Security)


## About the project:

This project documents the full **Footprinting & Scanning** of a simulated pentest within the **INE eJPT Skill Check Lab**.  

## Goal: 

The task was to gather *FLAGS (1 → 5)* using various reconnaissance tools and logical thinking, applying practical OSINT and scanning methods.


## Tools Used:

1. `Mozilla Firefox (Manual browsing)`
2. `Gobuster`
3. `DIRB`
4. `HTTrack`
5. `WhatWeb`
6. `Wget / Curl`
7. `Grep; md5sum`


## Results of Flags:


| Flags  | Task                                 | Hash / Value                                 | Method |
|--------|--------------------------------------|----------------------------------------------|--------|
| 1.     | robots.txt file                      | `2d4ea9ff30474660896a93bf2662bba3`           | Direct Access |
| 2.     | Web server & CMS version             | `38baf47279aa41fb9661cadd4bf20532`           | WhatWeb |
| 3.     | Directory listing                    | `a4bda9f806354b5d98fde9d200fc1fe8`           | DIRB |
| 4.     | Backup files discovery (403 error)   | **Not captured (403 Forbidden)**             | Gobuster + Curl |
| 5.     | Mirroring & API discovery            | `55574431357347bb843db2ddea9328`             | HTTrack + Grep |

## What i've noticed:

1. Discovered sensitive but inaccessible backup files (for example: `.bak`, `.sql`, `.zip`)
2. Encountered common tool errors (`gobuster + /dev/fd`) and solved via temp wordlists
3. Combined multiple tools
4. REST API endpoint revealed valid admin username (`admin`) for future attacks


## Access to the project:

*Written in Slovak language*

[EJPT Skill Check Lab.pdf](./EJPT%20Skill%20Check%20Lab.pdf)

## Author:

Bc. Peter Mulik **(mulcb0t)**

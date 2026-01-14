
# Bitsight Scanning infrastructure

BitSight is like that nosy neighbor who catches a glimpse of you through the blinds and suddenly thinks they know your whole life story. They’re constantly scanning the internet—crawling websites, peeking into open ports—to piece together how secure (or insecure) your digital setup is.</p>

But here’s the funny part: with just a few crumbs of data, they start extrapolating like there’s no tomorrow. Spot one open port? They assume your entire network security is looser than a thrift shop sweater. See a couple of outdated software versions? Suddenly, they’ve decided your entire IT department is running on Windows XP and duct tape.<br>
Before you know it, BitSight has slapped you with a cybersecurity score, rating your digital fortress like a strict schoolteacher grading a half-finished homework assignment.</p>

BitSight doesn’t just rate you based on what they find—they rate you on what they think they’ve found. And yes, they’re making wild guesses based on just a few hints, like assuming your whole house is a mess because they saw a sock on your porch.</p>

A smart approach? Think of it like staging your house for a real estate agent: show off only the clean, organized rooms and keep the messy closets out of sight. In other words, strategically manage what BitSight can see, making sure they walk away impressed by your well-maintained cybersecurity posture, rather than poking around for skeletons in your digital closets.</p>

## BitSight scanners: [link](https://github.com/vratiskol/Bitsight/blob/main/Bitsight_scanner_ips.txt)

45.156.128.0/22<br>
109.105.208.0/22<br>
185.117.225.0/24<br>
185.180.140.0/22<br>
<br>
2a10:3c0:1::/48<br>
2a10:3c0:2::/48<br>
2a10:3c0:3::/48<br>
2a10:3c0:4::/48<br>
2a10:3c0:5::/48<br>
2a10:3c0:100::/48<br>
2a10:3c0:101::/48<br>
2a10:3c0:102::/48<br>
2a10:3c0:200::/44<br>
<br>
Total IPv4: 3,328 IPs<br>
Total IPv6: 24×2<sup>80</sup><br>
<br>
### User-Agent used for Web scanning:

- User-Agent: Mozilla/5.0 (compatible; BitSightBot/1.0)
- User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.117 Safari/537.36
- User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/90.0.4430.212 Safari/537.36
<br>
<br>

# How does BitSight's "Compromised System" Category work?

**Netflix Mode: ON**
<p>:movie_camera: Imagine setting up a fake nightclub—complete with bouncers, flashing lights, and cheesy music—to catch all the party crashers who keep trying to get in with stolen invites. But, plot twist, just when they think they’ve snuck past the velvet rope and are ready to party, the doors swing open, and instead of a dance floor... they find themselves standing in a police station, under a spotlight, with officers ready to take notes on every move they’ve made.</p>

## BitSight Sinkholes:
<p>
    A sinkhole is like one of those "Gotcha!" traps. Hackers are using C2 with shady domains that act like their secret command centers.
    Once BitSight and other cybersecurity teams figure out these domains are being used for mischief, they swoop in, buy the domains, and turn them into bait.
</p>
<p>
    BitSight sets up fake servers that look just like the original botnet command centers (same open port). Now, when infected computers come knocking, expecting some juicy hacker commands, they get redirected to BitSight’s "honeypot."
    It’s like trying to enter a secret club, only to realize it’s actually the police station.
</p>

## Why Should You Care (or Not)?
<p>
    When a company’s computers start chatting with these domains, BitSight’s fake server takes note—like that bouncer jotting down the names of everyone trying to crash the party. The IP addresses in the connection logs are cross-checked with BitSight’s records to see which companies’ assets are getting a little too cozy with these shady domains.
</p>
<p>
    Now, if you find your company's IP on this list, don’t panic (yet). It is a strong hint that your cyber defenses might be about as sturdy as a wet paper bag.
    Sure, for now, it's just connecting to BitSight's sinkhole, but if a real hacker had been behind it, you’d be looking at a one-way ticket to Doomsville for your systems.
</p>

### BitSight Sinkhole IPs: [link](https://github.com/vratiskol/Bitsight/blob/2f1e16e4165094a700056345bbd8fd8e90abedd8/Bitsight_Sinkhole_ips.txt)

3.94.10.34<br>
3.83.187.118<br>
3.87.209.247<br>
3.215.174.86<br>
3.229.117.57<br>
3.238.30.69<br>
3.248.197.9<br>
3.249.135.232<br>
13.213.51.196<br>
13.214.182.154<br>
13.218.189.17<br>
18.142.91.111<br>
18.234.103.197<br>
18.236.80.58<br>
34.204.67.153<br>
34.219.29.107<br>
34.229.166.50<br>
34.234.66.220<br>
34.245.175.187<br>
44.192.103.96<br>
44.195.42.2<br>
44.247.155.67<br>
52.11.240.239<br>
52.26.80.133<br>
52.41.145.34<br>
52.43.119.120<br>
52.212.150.54<br>
54.85.87.184<br>
54.146.6.253<br>
54.157.23.253<br>
54.160.173.93<br>
54.169.144.97<br>
54.170.242.139<br>
54.174.115.238<br>
54.195.169.28<br>
54.251.193.134<br>
54.255.164.76<br>
63.32.168.222<br>
64.226.125.39<br>
178.79.170.240<br>
195.24.89.142<br>
2600:9000:2008:2a00:1:2317:a2c0:66ce<br>
2600:9000:201d:be00:e:2319:da00:e065<br>
2600:9000:201e:b800:1f:a793:8a00:bd70<br>
2600:9000:2021:2200:0:9e0c:5940:9c03<br>
2600:9000:2039:0:6:bb23:c280:32a7<br>
2600:9000:2039:e800:2:be37:2a00:93a1<br>

### Sinkhole Domains: [List of 97,342 domains](https://github.com/vratiskol/Bitsight/blob/2f1e16e4165094a700056345bbd8fd8e90abedd8/Bitsight_Sinkhole_list_domains.csv)


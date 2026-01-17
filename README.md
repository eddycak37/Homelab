# The Homelab Journey
In this part of the project, I will be explaining everything in details about my homelab

Table of contents
- Introduction
- Hardware
- Proxmox Virtual Environment
- Adguard Home
- Tailscale
- Home Assistant
- Nextcloud
- Future projects


# Introduction
To begin with, back in July 2025, I wanted to start working on a homelab using a used computer that I bought on Facebook Marketplace. I was planning to add a network add blocker, a self-hosting media softwares, a NAS and other things. 

Computer used: HP Prodesk 600 G3 SFF
- CPU: i5 something
- RAM: 32 Gb DDR4-2400 (I upgraded them)
- Storage: ADATA SSD SU650 240Gb
- Additional storage:
    - Seagate Barracuda SSD Q5 2TB
    - Crucial P310 SSD 1TB
    - Seagate Backup Plus Slim 2TB
    - Western Digital Black SN770 2TB
    - Western Digital Black SN850X 4TB

Here is the tree of my homelab at that time:
- Proxmox VE
    - Adguard Home
    - Nginx Proxy Manager
    - Cloudflared
    - Jellyfin
    - TrueNas
        - Arr Suites
        - Immich
        - QBittorrent
    - Tailscale
     
I won't lie, I was actually testing and trying different stuffs without knowing what I was doing. My adguard had too much Upstream DNS servers and it wasn't properly setup. For Nginx and Clouflared, I barely knew what to, but my goal was to access my homelab remotely. Jellyfin wasn't efficient. In my opinion, I should've just put it in TrueNas just like the Arr Suites in it. When it comes to TrueNas, if you look at my additional storage, I was using SSDs that I had before. A proper HDD setup in Raid would've been better because my Raid setup was quite special and I believe it was shortening my SSDs lifespan. It was storage in the SSDs pool with two USB sticks for cache and logs. The Arr Suites that I used was: Radarr, Sonarr, Configarr, Prowlarr and Bazarr. I had a lot of difficulties setting them together and get them to use my TrueNas storage. When it comes to other tools/softwares for downloads, I went with: Nzbgeek, QBittorrent and OpenSubtitles. Finally, to manage my photos and backing them up from all my devices, I used Immich. It was probably the most easiest one to setup in TrueNas. The one that I am most proud of finding and using is Tailscale. Really easy to setup and lot of cool features. So to keep it short:

- Network related
   - Adguard Home
   - Nginx Proxy Manager
   - Cloudflared
   - Tailscale
   - Dynu
- Media streaming
   - Arr suites
   - Jellyfin
- Storage
   - TrueNas
   - Immich

Now I will explain my journey about my new homelab that I started working on in January 2026. 

# Hardware
Computer used: Lenovo ThinkPad T480
- CPU: i5 8350u
- RAM: 16Gb DDR4-2400
- Storage: 256 Gb SSD
- Additional storage
   - Western Digital Black SN770 2TB on an external enclosure -> To use with my Nextcloud configuration
 
Now I invite you to go to my next repositories for the rest of my journey


  

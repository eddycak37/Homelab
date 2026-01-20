# The Homelab Journey
In this part of the project, I will be explaining everything in details about my homelab

## Table of contents
- Introduction
- Hardware
- Components


## Introduction
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

Here's the tree of my homelab at that time:
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
     
I won't lie, I was actually testing and trying different stuffs without knowing what I was doing. 

My Adguard had too much Upstream DNS servers and it wasn't properly setup. 

For Nginx and Clouflared, I barely knew what to, but my goal was to access my homelab remotely. After trying and searching for configurations, I came accross Tailscale. It was a lifesaver, but I believe it was still not properly configurated.

For my media streaming service, Jellyfin wasn't efficient. In my opinion, I should've just put it in TrueNas just like the Arr Suites in it. When it comes to TrueNas, if you look at my additional storage, I was using SSDs that I had before. A proper HDD setup in Raid would've been better because my Raid setup was quite special and I believe it was shortening my SSDs lifespan. It was storage in the SSDs pool with two USB sticks for cache and logs. 

The Arr Suites that I used was: Radarr, Sonarr, Configarr, Prowlarr and Bazarr. I had a lot of difficulties setting them together and get them to use my TrueNas storage. 

When it comes to other tools/softwares for downloads, I went with: Nzbgeek, QBittorrent and OpenSubtitles. 

Finally, to manage my photos and backing them up from all my devices, I used Immich. It was probably the most easiest one to setup in TrueNas. 

### To keep it short:

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

With all said, I was sceptical about how much the server was taking on my electricity bill. Having a full computer running 24/7 was maybe too much for Hydro-Québec and my wallet wouldn't be so happy about it. So I just dismantled everything. 

However, after some time, I came to realize I still wanted a homelab server, but I didn't wished for it to be too demanding. 

That's when I thought of using my ThinkPad. At first, I only thought of putting Adguard on it, but it came to me that I needed something like Dropbox or Google Drive. You see, I didn't wanted to pay for a subscription to have more storage, but having your files easily shareable between all your devices was something I really wanted. 

## Components

So for my new server, here are all the stuff that I put:
- Proxmox Virtual Environment -> Repository [Proxmox VE](https://github.com/eddycak37/Proxmox-VE)
- Adguard Home -> Repository [AdguardHome](https://github.com/eddycak37/AdguardHome)
- Tailscale -> Repository [Tailscale](https://github.com/eddycak37/Tailscale)
- Nextcloud -> Repository [Nextcloud](https://github.com/eddycak37/Nextcloud)
- Mealie -> Repository [Mealie](https://github.com/eddycak37/Mealie) 
 
<h1 align="center"> Now, I invite you to follow the links to my repositories for the rest of my journey</h1>

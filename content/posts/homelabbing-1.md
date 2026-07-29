---
date: '2026-04-10T15:22:56-05:00'
draft: false
title: 'Homelabbing'
---

I've been homelabbing for about a year now, and I think it’s going to be one of those hobbies that sticks with me for the rest of my life. For those who are uninitiated, homelabbing is the practice of experimenting with your own personal IT infrastructure. People go into homelabbing for a variety of reasons, whether it's to repurpose old hardware or take control of their digital life. 

I started doing it because I thought it would be hands-on way for me to learn real-world IT skills. 

# I used to be blind
Prior to homelabbing, I had a very oblivious relation to hardware. As a kid, I thought of computers more like phones: a new generation comes out every couple of years, and when your hardware started slowing down, that was just the machine telling you it was time to move on. Homelabbing has completely changed that relationship. Instead of passively living with technology, I’m learning from it and actively trying to improve it. 

# My personal sandbox
For instance, I turned my personal PC into a remote testing lab. By setting up secure remote access, I'm able to leverage my RTX 5070 Ti to experiment with GPU-heavy tasks from anywhere in the world. I regularly rely on this setup to handle computationally demanding assignments like in PHYS 235 or CS 540. Beyond schoolwork, having remote access to my GPU allows me to test out research projects, like running the recently released Depth Anything 3 models. Pushing my system with these kinds of state-of-the-art models has been incredibly eye-opening, because it forces me to understand the real-world limits of my current build and helps me pinpoint exactly what hardware capabilities I’ll need in order to tackle heavier workloads.

# My current setup
Instead of relying on a single all-in-one machine, I've built a modular homelab that splits tasks across a few specialized devices. By using Tailscale to link them together, my laptop essentially acts as a secure window into my entire setup, providing seamless control over all my machines no matter where I am. As someone who has dropped their fair share of laptops in the past, I find it very comforting that my most fragile, portable device is now just a replaceable access point, rather than the expensive brain of my entire operation. 

![My homelab setup](/images/setup.png)

### Hardware & Core Devices
* Laptop: Serves as my mobile command center. It allows me to securely manage, monitor, and interact with my entire setup whether I'm in a lecture hall or working remotely.
* Home Server: My primary compute engine, equipped with an RTX 5070 Ti. It is dedicated to running CUDA-based projects, training machine learning models, and testing heavy GPU workloads. [Setup](https://www.buildcores.com/builds/tvmXeHsTT?share=true)
* Mini PC: A low-power, always-on workhorse dedicated to hosting my personal website and managing lightweight microservices via Docker.

### Connectivity & Workflows
* Tailscale VPN: Forms the backbone of my private network, creating an encrypted, zero-configuration mesh between my laptop, server, and mini PC without exposing open ports to the public internet.
* RustDesk Remote Desktop: Gives me full graphical control over my home server when I need direct interface interactions from my laptop.
* VSCode Remote SSH: Enables me to code, debug, and execute scripts directly on my remote machines with ultra-low latency, keeping my local laptop lightweight and efficient.



# Proxmox Homelab Cluster

## Overview

This project documents my Proxmox homelab cluster used for learning virtualization, Linux administration, networking, and self-hosted services.

## Objectives

- Learn virtualization concepts
- Deploy and manage Linux VMs
- Configure cluster management
- Explore storage and backup solutions
- Host self-managed services

## Hardware

| Node | CPU | RAM | Storage |
|--------|--------|--------|--------|
| Node 1 | Intel I7 8700 | 16GB | 500GB SSD |
| Node 2 | Intel I9 13900KF | 64GB | 1TB SSD |

##setup

- Downloadeed Proxmox
  
Downloaded Proxmox ISO and flashed it on a usb with balena etcher. Booted from the USB to start the instaliation process.

- Instaliation process

  chose a drive to install the OS on. Selected the correct network and managment interface. Assigned a hostname, IP, gateway, and subnet. Review my selections and run the install.

  - Configuration
 
    Logged into my Proxmox web interface, disabled enterprise repositories, and added a no subscription repository. Used Proxmox post install script:
    
     [bash -c "$(curl -fsSL https://raw.githubusercontent.com/community-scripts/ProxmoxVE/main/tools/pve/post-pve-install.sh)"]

    Updated and restarted Proxmox.

## Issues and solutions

- Web interface not working

  Solutions: Ethernet was required and the IP was taken by another machine
  
## Cluster setup
    -
## Services

- Proxmox VE
- Docker
- Nextcloud
- Tailscale
- Linux VMs
- Post script -- https://community-scripts.org/scripts/post-pve-install

## Skills Demonstrated

- Linux Administration
- Virtualization
- Networking
- Troubleshooting
- Documentation

# Raspberry Pi 5 - Network Services Node

## Overview
The Raspberry Pi 5 serves as the primary network services node, handling DNS, VPN management, and mesh networking for the homelab.

## Hardware Specifications
- **Model**: Raspberry Pi 5
- **CPU**: Broadcom BCM2712 (ARM Cortex-A76 quad-core)
- **RAM**: [To be documented]
- **Storage**: [To be documented - SD card/USB]
- **Network**: Gigabit Ethernet + Wi-Fi 6

## Operating System
- **OS**: Raspberry Pi OS (Debian-based ARM64)
- **Installation Method**: [To be documented]
- **Boot Configuration**: [To be documented]

## Services Running

### Pi-hole
- **Purpose**: DNS ad-blocking and local DNS resolution
- **Port**: 80/443 (Web interface), 53 (DNS)
- **Configuration**: [To be documented]
- **Admin Interface**: http://[pi-ip]/admin

### WG Dashboard
- **Purpose**: WireGuard VPN management interface
- **Port**: [To be documented]
- **Configuration**: [To be documented]
- **Clients**: [To be documented]

### Tailscale
- **Purpose**: Exit node and subnet router for mesh VPN
- **Configuration**: Exit node enabled
- **Subnet Routes**: [To be documented]
- **Integration**: Provides secure access to homelab from anywhere

## Network Configuration
- **IP Address**: [To be documented]
- **VLAN**: [To be documented]
- **DNS Upstream**: [To be documented]
- **Port Forwards**: [To be documented]

## Security Considerations
- **SSH Access**: [To be documented]
- **Firewall Rules**: [To be documented]
- **Update Schedule**: [To be documented]

## Backup and Recovery
- **Backup Method**: [To be documented]
- **Restore Procedure**: [To be documented]
- **Configuration Backup**: [To be documented]

## Monitoring
- **Health Checks**: [To be documented]
- **Log Location**: [To be documented]
- **Alerts**: [To be documented]

## Troubleshooting
### Common Issues
- [To be documented as issues are encountered]

### Diagnostic Commands
```bash
# Pi-hole status
pihole status

# WireGuard interface status
wg show

# Tailscale status
tailscale status

# System resources
htop
df -h
```

## Future Enhancements
- [ ] Add more comprehensive monitoring
- [ ] Implement automated backups
- [ ] Consider redundancy setup

---
**Last Updated**: [Date]
**Responsible**: Network Team

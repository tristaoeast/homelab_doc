# Proxmox PVE - Minisforum BD795M

## Overview
The Minisforum BD795M serves as the primary virtualization host running Proxmox VE, providing compute resources for various VMs and services.

## Hardware Specifications
- **Model**: Minisforum BD795M
- **CPU**: [To be documented - AMD processor]
- **RAM**: [To be documented]
- **Storage**: [To be documented]
- **GPU**: NVIDIA GTX 1060 3GB (for VM passthrough)
- **Network**: [To be documented]
- **Power**: [To be documented]

## Proxmox VE Configuration
- **Version**: [To be documented]
- **Installation**: [To be documented]
- **Cluster**: Single node (potential for expansion)
- **Storage**: [To be documented - local/network storage]

## Virtual Machines

### HomeTower (Windows 11 VM)
- **Purpose**: Windows workstation/desktop VM
- **Resources**:
  - CPU: [To be documented]
  - RAM: [To be documented]
  - Storage: [To be documented]
- **GPU Passthrough**: NVIDIA GTX 1060 3GB
- **Use Cases**: [To be documented]

### Home Assistant OS VM
- **Purpose**: Smart home automation platform
- **Resources**:
  - CPU: [To be documented]
  - RAM: [To be documented]
  - Storage: [To be documented]
- **Network**: [To be documented]
- **Integrations**: Unifi Controller, various IoT devices

### Services in VMs

#### Nginx Proxy Manager
- **Location**: [VM or container - to be documented]
- **Purpose**: Reverse proxy and SSL certificate management
- **Configuration**: [To be documented]
- **Upstream Services**: [To be documented]

#### Unifi Controller
- **Location**: Running inside Home Assistant OS VM
- **Purpose**: Network device management
- **Integration**: Managed through Home Assistant
- **Devices**: [To be documented]

## GPU Passthrough Configuration
- **GPU**: NVIDIA GTX 1060 3GB
- **Target VM**: HomeTower (Windows 11)
- **Driver Configuration**: [To be documented]
- **Performance**: [To be documented]

## Network Configuration
- **Management Interface**: [To be documented]
- **VM Network**: [To be documented]
- **VLAN Configuration**: [To be documented]
- **Bridge Setup**: [To be documented]

## Storage Configuration
- **Local Storage**: [To be documented]
- **VM Storage**: [To be documented]
- **Backup Storage**: [To be documented]
- **ISO Storage**: [To be documented]

## Backup and Recovery
- **Backup Schedule**: [To be documented]
- **Backup Storage**: [To be documented]
- **Restore Procedures**: [To be documented]
- **VM Snapshots**: [To be documented]

## Monitoring and Maintenance
- **Resource Monitoring**: Proxmox web interface
- **Log Locations**: [To be documented]
- **Update Schedule**: [To be documented]
- **Health Checks**: [To be documented]

## Security
- **Access Control**: [To be documented]
- **Firewall**: [To be documented]
- **Certificate Management**: [To be documented]
- **SSH Access**: [To be documented]

## Performance Optimization
- **CPU Allocation**: [To be documented]
- **Memory Management**: [To be documented]
- **Storage Performance**: [To be documented]
- **Network Optimization**: [To be documented]

## Troubleshooting
### Common Issues
- [To be documented as issues are encountered]

### Diagnostic Commands
```bash
# Proxmox cluster status
pvecm status

# VM status
qm list

# Resource usage
pvesh get /nodes/[node]/status

# GPU passthrough status
lspci | grep NVIDIA

# VM configuration
qm config [vmid]
```

## Future Enhancements
- [ ] Cluster expansion (add more nodes)
- [ ] Shared storage implementation
- [ ] Enhanced backup solution
- [ ] Container workloads (LXC)
- [ ] Resource optimization

---
**Last Updated**: [Date]
**Responsible**: Virtualization Team

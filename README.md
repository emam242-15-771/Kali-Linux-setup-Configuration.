
# Kali Linux Attacker VM Setup — Oracle VirtualBox

A practical documentation project covering the setup, configuration, and verification of a Kali Linux attacker virtual machine using Oracle VirtualBox.

This repository documents the installation workflow, virtual machine settings, network configuration, post-installation tasks, and troubleshooting notes.

## Project Objectives

- Document the Kali Linux virtual machine setup process.
- Understand Oracle VirtualBox VM configuration.
- Explore NAT, Bridged Adapter, and Host-Only networking.
- Record post-installation configuration and verification steps.
- Maintain screenshots and reproducible lab documentation.
- Build a structured cybersecurity home lab for authorized security testing.

## Lab Environment

| Component | Configuration |
|---|---|
| Hypervisor | Oracle VirtualBox |
| Guest Operating System | Kali Linux |
| VM Role | Attacker Machine |

> Note: Replace the unspecified values with your actual VM configuration.

## Repository Structure

```text
Setting-Up-attacker-VM-Kali-Linux/
├── README.md
├── docs/
│   ├── installation.md
│   ├── network-configuration.md
│   ├── post-installation.md
│   └── troubleshooting.md
├── lab-notes/
│   └── verification-checklist.md
├── screenshots/
│   ├── virtualbox-manager.png
│   ├── vm-settings.png
│   ├── network-configuration.png
│   └── kali-desktop.png
└── scripts/
    └── setup-tools.sh
```

The structure above is the proposed organization for this project. Add files and screenshots as they become available.

## Setup Workflow

### 1. Download Kali Linux

- Visit the official Kali Linux website.
- Select an appropriate installation image.
- Verify the downloaded image using the official verification instructions.

Official resource: https://www.kali.org/get-kali/

### 2. Create the Virtual Machine

- Open Oracle VirtualBox Manager.
- Create a new virtual machine.
- Select the appropriate Linux operating system type.
- Allocate RAM and CPU resources according to the host system.
- Create a virtual hard disk.
- Attach the Kali Linux installation ISO.

### 3. Install Kali Linux

- Start the virtual machine.
- Follow the graphical installer.
- Configure the required locale, keyboard, user account, and storage options.
- Complete installation and restart the VM.
- Detach the installation ISO if required.

### 4. Configure Virtual Networking

VirtualBox provides different networking modes for different lab requirements.

| Mode | Typical Purpose |
|---|---|
| NAT | Outbound connectivity through the host |
| Bridged Adapter | Connect the VM to the physical network |
| Host-Only Adapter | Communication between the host and selected VMs |
| Internal Network | Communication between VMs on an isolated virtual network |

The appropriate mode depends on the lab topology and the required level of isolation.

For an isolated practice lab, use a suitable isolated network configuration and avoid exposing vulnerable lab machines to networks without authorization.

### 5. Post-Installation Configuration

Document the following tasks as they are completed:

- Confirm successful boot and login.
- Review display resolution and VM integration.
- Verify network connectivity.
- Check available disk space and system resources.
- Update packages using the appropriate Kali Linux procedure.
- Install only the tools needed for the intended lab.
- Record any configuration issues and their resolutions.

### 6. Verification

Use the checklist in `lab-notes/verification-checklist.md` to record each test, its result, and any observations.

Do not mark a test as successful until it has been performed.

## Screenshots and Evidence

Screenshots will document the actual configuration and installation process.

### VirtualBox Manager

![VirtualBox Manager](screenshots/virtualbox-manager.png)

### Virtual Machine Settings

![Virtual machine settings](screenshots/vm-settings.png)

### Network Configuration

![Network configuration](screenshots/network-configuration.png)

### Kali Linux Desktop

![Kali Linux desktop](screenshots/kali-desktop.png)

> Replace these image paths with your actual screenshot filenames. GitHub displays an image when the referenced file exists at the specified path.

## Documentation

- [Installation Guide](docs/installation.md)
- [Network Configuration](docs/network-configuration.md)
- [Post-Installation Notes](docs/post-installation.md)
- [Troubleshooting Guide](docs/troubleshooting.md)
- [Verification Checklist](lab-notes/verification-checklist.md)

These links will work once the corresponding files have been added to the repository.

## Troubleshooting Notes

Record problems encountered during the setup process, including:

- VM failing to boot
- Installation ISO not detected
- Network adapter disconnected
- No network connectivity inside Kali
- Insufficient allocated memory or storage
- Display resolution or integration issues

For each issue, document the observed symptoms, the diagnostic process, the verified solution, and any relevant screenshots.

## Security and Responsible Use

This repository documents a personal cybersecurity learning environment.

- Perform security testing only on systems you own or have explicit permission to assess.
- Keep intentionally vulnerable lab machines isolated where appropriate.
- Never commit passwords, private keys, API tokens, or sensitive network information.
- Sanitize screenshots before publishing them.
- Follow the licensing and redistribution requirements of included tools and software.

## References

- Kali Linux: https://www.kali.org/
- Kali Linux Documentation: https://www.kali.org/docs/
- Oracle VirtualBox: https://www.virtualbox.org/
- VirtualBox User Manual: https://www.virtualbox.org/manual/

## Project Status

**Status:** Documentation and lab setup project.

Additional configuration notes, verification evidence, and troubleshooting records will be added as the lab is developed.

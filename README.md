# Armbian for Rock Pi 4 SE

This repository provides a customized Armbian build tailored for the Radxa Rock Pi 4 SE single-board computer. It includes prebuilt images, kernel configurations, and build scripts optimized for the Rockchip RK3399 SoC.

## 🔧 Features

- Support for the Rock Pi 4 SE hardware  
- Optimized Linux kernel for Rockchip RK3399  
- Prebuilt Armbian images for quick deployment  
- Custom configurations and enhancements  

## 📦 Releases

You can find the latest prebuilt images under the [Releases](https://github.com/trappiz/armbian-rock4se/releases) section. For example, the `v25.5.0-trunk.426` release includes the most recent updates as of April 19, 2025.

## 🚀 Getting Started

### Prerequisites

- A Radxa Rock Pi 4 SE board  
- A microSD card or eMMC module (8GB or larger)  
- A computer with an SD card reader  

### Installation

1. Download the latest Armbian image from the [Releases](https://github.com/trappiz/armbian-rock4se/releases).  
2. Use a tool like [Balena Etcher](https://www.balena.io/etcher/) to flash the image onto your microSD card or eMMC module.  
3. Insert the storage device into your Rock Pi 4 SE board.  
4. Power on the board and allow it to boot into Armbian.  

### Initial Configuration

Upon first boot, you'll be prompted to complete the initial setup, including:

- Creating a new user account  
- Setting up the system locale and timezone  
- Configuring network settings  

For advanced configurations, use the `armbian-config` utility:

```bash
sudo armbian-config
```

This tool allows you to:
- Configure network interfaces
- Install additional software packages
- Manage system services
- Update the system firmware

## 🛠️ Building from Source

If you prefer to build the Armbian image yourself:
1. Clone the Armbian build framework:
```bash
git clone https://github.com/armbian/build.git
cd build
```

2. Start the build process:
```bash
./compile.sh
```

### 🧩 Customizations

This build includes:
- Updated device tree files for improved hardware compatibility
- Optimized kernel parameters for performance
- Pre-installed utilities for system monitoring and management

### 📚 Documentation

For comprehensive documentation on Armbian, visit the official Armbian documentation.

### 🤝 Contributing

Contributions are welcome! To contribute:
1. Fork the repository
2. Create a new branch for your feature or fix
3. Commit your changes with clear messages
4. Push your branch to your fork
5. Open a pull request detailing your changes

### 📄 License

This project is licensed under the GNU General Public License v2.0 (GPL-2.0).



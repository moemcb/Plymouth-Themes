# Amiga ROM 3.1 Plymouth Theme

A nostalgic Plymouth theme that recreates the classic Amiga Workbench 3.1 boot animation on modern Linux systems.  

## Preview

Amiga boot animation (normal version)  
![preview-normal](https://github.com/user-attachments/assets/your-screenshot-or-gif-here)

Amiga boot animation (zoomed version)  
![preview-zoomed](https://github.com/user-attachments/assets/your-screenshot-or-gif-here)

## Features

- Recreation of the original Amiga 3.1 ROM boot screen
- Two variants included:
  - **Normal**  
  - **Zoomed** 
- Separate animations for boot and shutdown

## Installation

```bash
# 1. Pick your flavor and copy the frames
# Normal version
sudo cp -r frames.normal/* amiga-rom-3-1/frames/

# OR zoomed
sudo cp -r frames.zoomed/* amiga-rom-3-1/frames/

# 3. Install the theme
sudo cp -r amiga-rom-3-1 /usr/share/plymouth/themes/

# 4. Make it the default
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/amiga-rom-3-1/amiga-rom-3-1.plymouth 100
sudo update-alternatives --config default.plymouth

# 5. Regenerate initramfs
sudo update-initramfs -u

# 6. Reboot
sudo reboot
```

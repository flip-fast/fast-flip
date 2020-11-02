# Enable Wayland on Ubuntu
Execute below steps on Ubuntu Desktop but not via remote ssh
Open /etc/gdm3/custom.conf and ensure WaylandEnable=false is commented.
Logout and click on the gear button and select option "Ubuntu on Wayland"
once booted to desktop, make sure "echo $WAYLAND_DISPLAY" = wayland-0.

## Quickstart
To build your system, you will need to follow these instructions:
1. Clone Bootstrap project:
```bash
git clone https://github.com/flip-fast/bootstrap.git
```
2. Clone source code:
```bash
 ./sync_code.sh
```
3. Install all system dependencies:
```bash
./tools/install_system_dependencies.sh
```
4. Fetch the code:
```bash
./sync_code.sh
```
5. Kick off the build of the container and generate
a rootfs image using the default settings. 
```bash
./build.sh --rebuild-all
```
6. Check build/launch/README.md for instructions to run the VM and container.

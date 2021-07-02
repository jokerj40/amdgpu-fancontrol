# amdgpu-fancontrol

Simple bash script to control AMD Radeon graphics cards fan pwm forked from [here](https://github.com/grmat/amdgpu-fancontrol). Adjust temp/pwm values and hysteresis/interval in the script as desired. Other adjustments, such as the correct hwmon path might be required as well.

This script was initially meant as an example. Please don't just run it naively and keep in mind that I'm not responsible for failures.

---

I added simple OpenRC service script. Copy `amdgpu-fancontrol` script to `/usr/bin` directory. Copy OpenRC service from `service/amdgpu-fancontrol` to `/etc/init.d` directory. Copy config to `/etc/amdgpu-fancontrol.cfg`. Enable service at startup: `rc-update add amdgpu-fancontrol default`.

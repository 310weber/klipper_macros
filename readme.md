##Setup instructions:

1.  SSH to printer and run the following commands:

`cd ~/printer_data/config`

`git clone https://github.com/310weber/klipper_macros.git`

2. Edit 'macros.cfg' to (un)comment macros to enable/disable them.

3. Add the following to 'moonraker.cfg' to enable automatic updates.
```
[update_manager Klipper_Macros]
type: git_repo
channel: dev
path: ~/printer_data/config/klipper_macros
origin: https://github.com/310weber/klipper_macros.git
managed_services: klipper
primary_branch: main
```
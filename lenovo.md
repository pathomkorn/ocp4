# OpenShift 4 Installation - Bare Metal Node on Lenovo PC

* You may have to remove kernel argument `console=ttyS0,115200n8`
* DHCP is required for using `--delete-karg` parameter for `coreos-installer`
* Run `coreos-installer` command with `--delete-karg console=ttyS0,115200n8` parameter

```bash
coreos-installer install /dev/sda --ignition_url http://${WEBSERVER}/worker1.ign --delete-karg console=ttyS0,115200n8 
```

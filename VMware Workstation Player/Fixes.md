# Errors and Fixes

### Errorr
```
error = "Could not connect 'Ethernet0' to virtual network '/dev/vmnet8'. More information can be found in the vmware.log file. Failed to connect virtual device 'Ethernet0'." from vmware workstation player on ubuntu 25
```

### Fix
```
1. stop VMware Workstation Player
2. Rebuild vmware kernel modules (vmnet, vmmon)
sudo vmware-modconfig --console --install-all
3. restart VMware

```
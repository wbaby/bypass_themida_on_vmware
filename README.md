## bypass_themida_on_vmare

# Edit virtual machine's *.vmx* file with the following lines:
```
svga.vramSize = 268435456
monitor_control.restrict_backdoor = "TRUE"
monitor_control.disable_directexec = "TRUE"
isoliation.tools.getPtrLocation.disable = "TRUE"
isoliation.tools.setPtrLocation.disable = "TRUE"
isoliation.tools.getVersion.disable = "TRUE"
SMBIOS. reflectHost = "TRUE"
```

# Edit regedit of virtual machine
- Locate `HKEY_LOCAL_MACHINE/SYSTEM/CurrentControlSet/Control/Class/{4D36E968-E325-11CE-BFC1-08002BE10318}/0000`
- Set `DriverDesk` value to `ATI/NDIDIA SVGA II`

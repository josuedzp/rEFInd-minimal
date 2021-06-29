## Install rEFInd on Windows

 1. Download rEFInd (download zip) [here](https://sourceforge.net/projects/refind/files/)

 2. Extract zip

 3. Mount EFI partition:
 
    ```PS > mountvol S: /s```

 4. Copy refind folder into EFI partition `PS > xcopy \E refind S:\EFI\refind`

 4. Set rEFInd as default EFI `PS > bcdedit /set "{bootmgr}" \EFI\refind\refind_x64.efi`

## Install rEFInd on Linux

### Ubuntu

  ` $ sudo apt-get install refind `

### Fedora
 1. Download rEFInd (download rpm) [here](https://sourceforge.net/projects/refind/files/)
 2. `$ sudo dnf install ./refind.rpm`


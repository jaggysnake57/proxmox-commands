## adding disks

```bash
ls -al /dev/disk/by-id | grep ZR168QB7

qm set 236 -scsi1 /dev/disk/by-id/ata-ST8000DM004-2U9188_ZR165YGX
qm set 236 -scsi2 /dev/disk/by-id/ata-ST8000DM004-2U9188_ZR164FL3
qm set 236 -scsi3 /dev/disk/by-id/ata-ST8000DM004-2U9188_ZR168QB7
```

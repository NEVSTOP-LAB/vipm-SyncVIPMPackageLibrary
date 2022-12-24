# vipm-SyncVIPMPackageLibrary

use [lvcicd:vipm_syncvipmpackagelibrary](https://github.com/LV-APT/lvCICD/blob/main/docs/Operation-List.md#vipm_syncvipmpackagelibrary-sync-vipm-package-over-network) to sync vipm repo over network.

How to Use it:

```
      - name: SyncVIPMPackageLibrary
        id: build-vip
        uses: NEVSTOP-LAB/vipm-SyncVIPMPackageLibrary@main
        with:
          LabVIEW_Version: 2017
```

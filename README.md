# vipm-SyncVIPMPackageLibrary

use [lvcicd:BuildDailyVIP](https://github.com/LV-APT/lvCICD/blob/main/docs/Operation-List.md#vipm_buildvipackage--build-vipm-library) to sync vipm repo over network.

How to Use it:

```
      - name: SyncVIPMPackageLibrary
        id: build-vip
        uses: NEVSTOP-LAB/vipm-SyncVIPMPackageLibrary@main
        with:
          LabVIEW_Version: 2017
```

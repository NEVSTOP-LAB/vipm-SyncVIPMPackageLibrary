# vipm-BuildViPackage

use [lvcicd:BuildDailyVIP](https://github.com/LV-APT/lvCICD/blob/main/docs/Operation-List.md#vipm_buildvipackage--build-vipm-library) to build vipm package.

How to Use it:

```
      # Runs a set of commands using the runners shell
      - name: BuildDailyVIP
        id: build-vip
        uses: NEVSTOP-LAB/vipm-BuildViPackage@main
        with:
          LabVIEW_Version: 2017
          VipbPath: ${{ github.workspace }}

      - name: Upload a Build Artifact
        uses: actions/upload-artifact@v3.0.0
        with:
          # Artifact name
          name: ${{ steps.build-vip.outputs.vipName }}
          path: ${{ steps.build-vip.outputs.vipPathName }}
          # The desired behavior if no files are found using the provided path.
          if-no-files-found: warn
          retention-days: 90
```

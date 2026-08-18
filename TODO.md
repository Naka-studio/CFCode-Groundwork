# CF Code - Project TODO

## Phase 1 - Restrukturisasi

### Pending
- [ ] Rename plugin ID dari `com.foxdebug.acode.rk.*` ke `com.nakastudio.cfcode.*`
  - plugincontext
  - proot
  - customtabs

## Phase 2 - Feature Development
- [ ] Git Integration (sidebar + page)

## Notes
- Plugin di `src/plugins/` sementara masih pake ID Acode, rename belakangan
- Build via GitHub Actions (Nightly Release workflow)
- Package ID: com.nakastudio.coffeecode

## Cordova Plugins - Pending Cleanup
- [ ] browser/utils/updatePackage.js - Java package paths masih foxdebug
- [ ] system/utils/changeProvider.js - masih referensi com.foxdebug

## src/ui/pages/ - Pending Rename/Refactor
- [ ] plugin/ → rename ke extension/ (sesuai naming CF Code)
- [ ] plugins/ → rename ke extensions/ (sesuai naming CF Code)
- [ ] runningProcesses/ → pertimbangkan pindah ke ui/panels/

## shared/utils/general/
- [ ] apiInterceptor.js — ganti URL acode.app/api ke CF Code API endpoint waktu backend udah ready

## src/styles/
- [ ] overrideAceStyle.scss — review apakah masih relevan, CF Code pake CodeMirror bukan Ace

## src/tests/
- [ ] ace.test.js — review apakah masih relevan atau perlu ditulis ulang untuk CodeMirror

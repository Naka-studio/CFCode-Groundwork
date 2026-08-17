# Migration Map: Acode → CF Code

## src/lib/ → 

### src/core/editor/
- editorManager.js
- editorFile.js
- selectionMenu.js
- customTab.ts

### src/core/filesystem/
- fileIndex.js
- fileList.js
- fileTypeHandler.js
- checkFiles.js
- openFile.js
- openFolder.js
- saveFile.js
- remoteStorage.js

### src/core/commands/
- commands.js
- keyBindings.js

### src/core/workspace/
- projects.js
- recents.js
- saveState.js
- restoreFiles.js

### src/core/search/
- searchHistory.js

### src/services/settings/
- settings.js
- applySettings.js
- config.js
- systemConfiguration.js

### src/services/language/
- lang.js
- languageModeRecommendations.js

### src/services/theme/
- restoreTheme.js
- fonts.js

### src/services/plugin/
- installPlugin.js
- loadPlugin.js
- loadPlugins.js
- checkPluginsUpdate.js
- installState.js

### src/services/notification/
- notificationManager.js

### src/services/analytics/
- adConsentCoordinator.mjs
- adRewardBannerPolicy.mjs
- adRewards.js
- bannerVisibilityController.mjs
- privacyChoicesController.mjs
- secureAdRewardState.js
- startAd.js
- removeAds.js

### src/extensions/api/
- acode.js

### src/modules/formatter/
- prettierFormatter.js
- registerPrettierFormatter.js

### src/platform/android/
- webview.js
- run.js

### src/shared/utils/general/
- ajax.js
- polyfill.js
- lazyImports.js
- logger.js
- devTools.js

### src/shared/
- auth.js

### src/ui/components/
- showFileInfo.js

### src/ui/panels/
- console.js

---

## src/cm/ → src/editor/codemirror/
## src/components/ → src/ui/components/
## src/pages/ → src/ui/pages/
## src/dialogs/ → src/ui/dialogs/
## src/sidebarApps/ → src/ui/sidebar/
## src/palettes/ → src/ui/palettes/
## src/settings/ → src/services/settings/
## src/lang/ → src/locales/
## src/res/ → src/assets/
## src/handlers/ → tersebar (lihat mapping per file)
## src/fileSystem/ → src/core/filesystem/
## src/theme/ → src/services/theme/
## src/utils/ → src/shared/utils/
## src/views/ → src/views/
## src/plugins/ → src/extensions/

## Koreksi Mapping

### src/fileSystem/
- ftp.js, sftp.js → src/core/filesystem/ (capability, bukan platform-specific)
- externalFs.js, internalFs.js → src/platform/android/filesystem/ (Android Storage Access)

### src/handlers/
- purchase.js → src/services/purchase/ (domain tersendiri)
- windowResize.js → src/ui/layout/ (UI concern, bukan platform-specific)

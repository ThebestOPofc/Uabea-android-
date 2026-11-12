# English UI Translation Notes

This source package contains an English translation of the Android-facing UABEA interface and user-visible messages.

## Updated

- Android main screen, action buttons, prompts, overlays, and search/filter dialogs.
- File and folder picker labels, navigation controls, and file-picker error messages.
- Asset information, TypeTree, raw/dump import, and Mesh preview messages.
- Texture2D and TextAsset preview/replacement messages.
- Import/export, save, compression, rename, delete, and status/log messages.
- Settings titles and descriptions in `UABEA.Core/Config/ConfigurationManager.cs`.
- Android storage-permission feedback and crash-report text.
- Duplicate-file and plugin service error messages shared with the Android build.

## Scope and validation

Only user-facing strings were translated; program logic, asset serialization behavior, plugin APIs, and file formats were not intentionally changed. Chinese developer comments and internal design documents remain as they were because they do not appear in the app UI.

The XAML/XML files were parsed successfully. A .NET SDK is not installed in the editing environment, so an Android APK build could not be run here. Build and test the project with the .NET 8 Android workload before installing it on a device.

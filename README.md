# appimage-builder-flutter-example

This project aims to ilustrate how to pack a [flutter](https://flutter.dev) project into an AppImage. Also includes
as a bonus the instructions for setting un a CI workflow using Github Actions.

## Requirementes
- Ubuntu (18.04 or higher)
- [flutter](https://flutter.dev/docs/get-started/install/linux)
- [appimage-builder](https://appimage-builder.readthedocs.io/en/latest/intro/install.html)

## Build

```
git clone https://github.com/AppImageCrafters/appimage-builder-flutter-example.git
cd appimage-builder-flutter-example

# enable flutter desktop support
flutter channel dev
flutter upgrade
flutter config --enable-linux-desktop

# build the flutter app
flutter build linux

# build the AppImage
appimage-builder --skip-test
```


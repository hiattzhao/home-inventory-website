# Downloads Folder

Place your distribution files here:

## Linux

- `home-inventory-app_1.0.0-1_all.deb` - Debian/Ubuntu package
- `Home_Inventory_Manager.AppImage` - Universal Linux AppImage

## Windows

- `Home Inventory Manager.exe` - Windows installer or executable

## Building the packages

### Linux (.deb)

```bash
cd ../home-inventory-app
./build_debuild.sh
cp ../home-inventory-app_1.0.0-1_all.deb ../home-inventory-website/downloads/
```

### Linux (AppImage)

```bash
cd ../home-inventory-app
./build_appimage.sh
cp dist/Home_Inventory_Manager.AppImage ../home-inventory-website/downloads/
```

### Windows

Use PyInstaller on Windows to create the executable, or cross-compile if possible.

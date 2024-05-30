# NOTES

https://support.monotype.com/en/articles/7859096-syncing-and-installing-fonts-with-the-monotype-app



OLD
<key>SEARCH_PATTERN</key>
<string>https://monotypeapp.monotype.com/release/\d+/mac/system/DTAppInstaller.pkg.zip</string>

NEW
<key>SEARCH_PATTERN</key>
<string>https://monotypeapp.monotype.com/release/\d+/mac/MTFInstaller.zip</string>

https://monotypeapp.monotype.com/release/710/mac/MTFInstaller.zip


# SILENT UNINSTALL IF NEEDED
sudo /Applications/Monotype\ Fonts/.Components/Services/CoreServices/MonotypeFontsService --uninstaller
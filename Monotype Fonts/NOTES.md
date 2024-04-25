
https://support.monotype.com/en/articles/7859096-syncing-and-installing-fonts-with-the-monotype-app



OLD
<key>SEARCH_PATTERN</key>
<string>https://monotypeapp.monotype.com/release/\d+/mac/system/DTAppInstaller.pkg.zip</string>

NEW
<key>SEARCH_PATTERN</key>
<string>https://monotypeapp.monotype.com/release/\d+/mac/MTFInstaller.zip</string>

https://monotypeapp.monotype.com/release/710/mac/MTFInstaller.zip


        <dict>
            <key>Processor</key>
            <string>FlatPkgUnpacker</string>
            <key>Arguments</key>
            <dict>
                <key>flat_pkg_path</key>
                <string>%RECIPE_CACHE_DIR%/unzip/MTFInstaller.pkg</string>
                <key>destination_path</key>
                <string>%RECIPE_CACHE_DIR%/unpkg/</string>
                <key>purge_destination</key>
                <true/>
            </dict>
        </dict>
        

  - Processor: FlatPkgUnpacker
    Arguments:
        flat_pkg_path: "%RECIPE_CACHE_DIR%/unzip/MTFInstaller.pkg"
        destination_path: "%RECIPE_CACHE_DIR%/unpkg/"
        purge_destination: false
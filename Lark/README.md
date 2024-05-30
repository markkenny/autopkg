# NOTES
Recipe no longer in se by owner.


https://www.larksuite.com/download

https://www.larksuite.com/api/downloads


https:\/\/.*\/Lark-darwin_arm64-.*signed.dmg

https:\/\/.*\/Lark-darwin_%DOWNLOAD_ARCH*-.*signed.dmg

https:\/\/sf16-va.larksuitecdn.com\/obj\/lark-artifact-storage\/dbd15936.*\/Lark-darwin_arm64-.*.dmg


(?P<url>https://*/Lark-darwin_arm64-.*.dmg).*Apple



https://regex101.com/

https://github.com/autopkg/autopkg/wiki/Processor-URLTextSearcher

https://regexlearn.com/



		<dict>
			<key>Arguments</key>
			<dict>
				<key>dmg_path</key>
				<string>%pathname%</string>
			</dict>
			<key>Processor</key>
			<string>AppDmgVersioner</string>
		</dict>
		<dict>
			<key>Arguments</key>
			<dict>
				<key>pkgdirs</key>
				<dict>
					<key>Applications</key>
					<string>0775</string>
				</dict>
				<key>pkgroot</key>
				<string>%RECIPE_CACHE_DIR%/%NAME%</string>
			</dict>
			<key>Processor</key>
			<string>PkgRootCreator</string>
		</dict>
		<dict>
			<key>Arguments</key>
			<dict>
				<key>destination_path</key>
				<string>%pkgroot%/Applications/Lark.app</string>
				<key>source_path</key>
				<string>%pathname%/Lark.app</string>
			</dict>
			<key>Processor</key>
			<string>Copier</string>
		</dict>
		<dict>
			<key>Arguments</key>
			<dict>
				<key>pkg_request</key>
				<dict>
					<key>chown</key>
					<array>
						<dict>
							<key>group</key>
							<string>admin</string>
							<key>path</key>
							<string>Applications</string>
							<key>user</key>
							<string>root</string>
						</dict>
					</array>
					<key>id</key>
					<string>%bundleid%</string>
					<key>options</key>
					<string>purge_ds_store</string>
					<key>pkgdir</key>
					<string>%RECIPE_CACHE_DIR%</string>
					<key>pkgname</key>
					<string>%NAME%-%ARCHITECTURE%-%version%</string>
				</dict>
			</dict>
			<key>Processor</key>
			<string>PkgCreator</string>
		</dict>

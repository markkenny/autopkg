# NOTES


         <dict>
            <key>Processor</key>
            <string>PathDeleter</string>
            <key>Arguments</key>
            <dict>
               <key>path_list</key>
               <array>
                  <string>%RECIPE_CACHE_DIR%/downloads/unpack</string>
                  <string>%RECIPE_CACHE_DIR%/downloads/payload</string>
               </array>
            </dict>
         </dict>


         		<dict>
				<key>destination_path</key>
				<string>%RECIPE_CACHE_DIR%/expanded</string>
				<key>pkg_payload_path</key>
				<string>%RECIPE_CACHE_DIR%/unpacked/Topaz_Photo AI.pkg/payload</string>
				<key>purge_destination</key>
				<true/>
			</dict>



		<dict>
			<key>Processor</key>
			<string>PathDeleter</string>
			<key>Arguments</key>
			<dict>
				<key>path_list</key>
				<array>
					<string>%RECIPE_CACHE_DIR%/expanded</string>
					<string>%RECIPE_CACHE_DIR%/unpack</string>
				</array>
			</dict>
		</dict>

[OpenWebStart settings](https://openwebstart.com/configuration/) are configurable with a response.varfile. Modify the varfile to match preferred settings before building the package.

Postinstall script runs an [unattended install](https://openwebstart.com/installation/) to configure settings in response.varfile, and then clean up install files.

Codesignature verificaton

<dict>
    <key>Arguments</key>
    <dict>
        <key>requirement</key>
        <array>
            <string>Developer ID Installer: Karakun AG (M975RKD6AX)</string>
            <string>Developer ID Certification Authority</string>
            <string>Apple Root CA</string>
        </array>
        <key>input_path</key>
        <string>%pathname%/OpenWebStart\ Installer.app</string>
    </dict>
    <key>Processor</key>
    <string>CodeSignatureVerifier</string>
</dict>
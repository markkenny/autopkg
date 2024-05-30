# NOTES


https://github.com/autopkg/homebysix-recipes/blob/451116206a2e4749a5ccf978f14ef3d30068d441/Amazon/AWSCLI.download.recipe

	<array>
		<dict>
			<key>Processor</key>
			<string>URLDownloader</string>
			<key>Arguments</key>
			<dict>
				<key>url</key>
				<string>https://awscli.amazonaws.com/AWSCLIV2.pkg</string>
			</dict>
		</dict>
		<dict>
			<key>Processor</key>
			<string>EndOfCheckPhase</string>
		</dict>
		<dict>
			<key>Processor</key>
			<string>CodeSignatureVerifier</string>
			<key>Arguments</key>
			<dict>

			</dict>
		</dict>
	</array>


DistributionPkgInfo
https://github.com/autopkg/dataJAR-recipes/tree/master

https://github.com/autopkg/dataJAR-recipes/tree/master/Shared%20Processors

https://github.com/autopkg/n8felton-recipes/blob/master/SharedProcessors/PkgInfoVersioner.py

https://github.com/autopkg/nmcspadden-recipes/blob/master/Shared_Processors/PackageInfoVersioner.py
https://github.com/autopkg/autopkg/blob/master/Code/autopkglib/PkgInfoCreator.py
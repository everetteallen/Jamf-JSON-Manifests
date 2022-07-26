# Jamf-JSON-Manifests

Here are a few Jamf JSON format configuration profile manifests that folks may find helpful.  I have not added these to the Profile Manifest Mirror (https://github.com/Jamf-Custom-Profile-Schemas/ProfileManifestsMirror) because I am writing these directly in JSON which is easier for me.  To use these Custom JSON schema see Eliot Jordan's excellent post at https://www.elliotjordan.com/posts/profilemanifestsmirror/

## 1) com.twocanoes.xcreds
This is an example JSON manifest template for the Twocanoes XCreds software (https://twocanoes.com/products/mac/xcreds/) which implements Cloud Login and password sync for macOS. Remember to remove empty properties that will not be set when imported into Jamf Pro.

## 2) jamf-vars-manifest
While searching for a sane way to report by Site (no Jamf does not expose this) I saw this page https://macnotes.wordpress.com/2022/01/14/device-specific-parameters-for-jamf-pro-script-policies/
on using configuration profiles to make the values of Jamf Variables (https://docs.jamf.com/jamf-pro/administrator-guide/Computer_Configuration_Profiles.html) available to scripts using the /usr/bin/defaults command line tool.  I created a JSON template for a macOS configuration profile that has all the Jamf Variable pre-populated.  NOTE: for EXTENTIONATTRIBUTE_# the number will need to be added to the string like EXTENTIONATTRIBUTE_1.  The Jamf Pro web interface allows adding attributes to the custom schema.
  
  

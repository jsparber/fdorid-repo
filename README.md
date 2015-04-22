# fdorid-repo
My own fdroid repo

###Add apk to the repo
create a dir with all apks.

###Create a repo without fdroidserver, used only jarsigner
Put the index.xml file in a zip and rename it to index.jar and move it to the apk.

#####Create a keystore
    keytool -genkey -alias alias-name -keystore keystore-name
#####Sign jar
    jarsigner -keystore keystore-name -storepass keystore-password -keypass key-password index.jar alias-name
    

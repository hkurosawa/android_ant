* Adding ant script to the Android project

1. create Android Project from Eclipse
2. copy build.xml, ant.properties and local.properties to project root directory
3. edit local.properties to point to the android sdk


* Signing App using Ant

1. edit ant.properties to point to your keystore file and alias name
2. then '$ ant release' will prompt you to imput the password withing build process
[reference] http://developer.android.com/guide/publishing/app-signing.html


* Generating keystore from command line

keytool -genkey -v -keystore my-release-key.keystore -alias alias_name -keyalg RSA -keysize 2048 -validity 10000 

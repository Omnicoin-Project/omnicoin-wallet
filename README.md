<div align="center"><h1>Welcome to <b>Omnicoin Wallet</b></h1></div>

<div align="center">A standalone omnicoin payment app for your Android device!</div>


<div align="center"><img src="https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcT5cGH94w6MbLPaBojOdBAVmPM9pbqJm3LIn2gNd4tPKd1F8qbgmg" /></div>

<div align="center">Visit the <a href="https://github.com/Omnicoin-Project/Omnicoin/wiki">Omnicoin Wiki</a> for more information</div>


<br />
This project contains several sub-projects:

 * __wallet__:
     The Android app itself. This is probably what you're searching for.
 * __market__:
     App description and promo material for the Google Play app store.
 * __integration-android__:
     A tiny library for integrating omnicoin payments into your own Android app
     (e.g. donations, in-app purchases).
 * __sample-integration-android__:
     A minimal example app to demonstrate integration of omnicoin payments into
     your Android app.

<br />

### COMPILATION INSTRUCTIONS
1. Clone the git repository <code>git clone https://github.com/MeshCollider/omnicoin-wallet.git</code>
2. Make sure you have the Java Development Kit (JDK) and Maven version 3.0.5 installed and in your path, and make sure JAVA_HOME is set to your JDK root directory.
3. Download the android SDK and make sure you download the necessary API level versions for the wallet
4. Compile the wallet with this command executed inside the omnicoin-wallet directory, where ../../android-sdk is replaced with the path to your android SDK: <code>mvn clean install -Dandroid.sdk.path=../../android-sdk -DskipTests</code>
5. The APK file will then be found in wallet/target directory.
6. 
### SIGNING THE APK FILE
1. Run <code>jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore omnicoin-wallet-keystore.keystore wallet-unsigned.apk Omnicoin</code> where omnicoin-wallet-keystore.keystore is the keystore, and wallet-unsigned.apk is the unsigned APK file, and Omnicoin is the alias name from your keystore.
2. Align the APK with: <code>zipalign -v 4 wallet-signed.apk wallet.apk</code>

Developed by MeshCollider. See AUTHORS for credits.

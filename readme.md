

sample.keystore is at Sample/app/sample.keystore

https://github.com/saxenajabong/Sample/blob/master/app/sample.keystore


1. alias bundletool='java -jar ~/Desktop/installers/bundletool-all-0.5.0.jar'

2. bundletool build-apks --connected-device --bundle=/Users/prabhooji/Desktop/Sample/app/release/app.aab --output=~/sample.apks --ks=/Users/prabhooji/Desktop/Sample/app/sample.keystore --ks-pass=pass:sample --ks-key-alias=Sample --key-pass=pass:sample

3. $ANDROID_HOME/extras/google/instantapps/ia --debug run /Users/prabhooji/Desktop/Sample/sample/splits/*.apk

4. keytool -list -v -keystore sample.keystore -alias Sample -storepass sample -keypass sample
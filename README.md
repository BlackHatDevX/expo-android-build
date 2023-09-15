# expo-android-build
react native guide to build expo apps using eas locally
```
wget https://download.oracle.com/java/17/latest/jdk-17_linux-x64_bin.deb
sudo apt-get -qqy install ./jdk-17_linux-x64_bin.deb
sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-17-oracle-x64/bin/java 1919
```

```
npm install -g eas-cli
apt-get install android-sdk
export ANDROID_HOME=/usr/lib/android-sdk
```

```
sudo wget https://dl.google.com/android/repository/commandlinetools-linux-10406996_latest.zip
sudo unzip commandlinetools-linux-10406996_latest.zip -d cmdline-tools
sudo mkdir --parents "$ANDROID_HOME/cmdline-tools/latest"
sudo mv cmdline-tools/* "$ANDROID_HOME/cmdline-tools/latest/"
export PATH=$ANDROID_HOME/cmdline-tools/latest/bin:$PATH
```
```
sudo apt install sdkmanager
sudo yes | sdkmanager --licenses
eas build --local
```

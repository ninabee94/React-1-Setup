# React-1-Setup

<b>1. Install chocolatey in cmd admin</b>

     Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
 
     
     // type 'choco' to check
     
<b>2. Install node.js, python2 & jdk8 in cmd admin</b>
     
     choco install -y nodejs.install python2 jdk8
     
<b>3. Download & install Android Studio</b>
 
     https://developer.android.com/studio
     
<b>4. Install platform and build tool</b>

     open android studio ==> tools ==> sdk tools ==> Android SDK     
     
     ==> sdk platforms : install Android SDK Platform 28 & Google APIs Intel x86 Atom System Image
     ==> sdk tools : install build tools 28
     
<b>5. Setup Android Home & platform-tools in environment variables</b>

<b>6. Create new react native project</b>
  
     react-native init AwesomeProject
     
<b>7. Setup for deployment</b>
  
     Option 1: run in avd
     
          open ./AwesomeProject/android in android studio
          open avd icon (top right)
          create new avd with api 28
          install haxm if needed
          
     
     Option 2: run in device
     
          enable phone usb debugging
          connect phone & computer to usb
          type 'adb devices' in cmd to check device name (eg: VXXNU19509200029)
          
          
<b>8. Run project in cmd</b>

     react-native run-android

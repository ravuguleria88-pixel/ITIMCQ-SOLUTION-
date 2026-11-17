# ITI MCQ Solution — Android APK Package

App Name: ITI MCQ Solution
Developer: Ravi Guleria, Instructor COPA
Target Web App URL: https://ais-pre-jucpaveh564kkf7uvjro5a-106422717684.asia-northeast1.run.app

## Option 1: Build APK Locally (Requires Node 18+ & JDK 17)
1. Install Bubblewrap CLI:
   npm install -g @bubblewrap/cli
2. Generate signing keystore:
   keytool -genkeypair -v -keystore android.keystore -alias iti-mcq-key -keyalg RSA -keysize 2048 -validity 10000
3. Update & build signed APK:
   bubblewrap update --manifest=./twa-manifest.json
   bubblewrap build

## Option 2: Zero-Setup Build via GitHub Actions
1. Upload this extracted folder to a GitHub repository.
2. Open the Actions tab and run "Build Signed Android APK".
3. Download the compiled ITI-MCQ-Solution.apk artifact.

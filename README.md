Demo of expo-dev-client crash on SDK 49 in dev builds without hermes. This demo uses react-native-v8.

Issue: When using a JS engine other than hermes expo-dev-client crashes on startup in dev builds on SDK 49

To reproduce:

1. `eas build -p android --profile development --local`
2. install APK on device or sim
3. `npx expo start`
4. load app on device
5. observe crash `couldn't find libhermes.so`

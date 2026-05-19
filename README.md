# Expo Asset - Issue Example

## Steps
- `npx create-expo-app@latest`
- `npx expo install expo-asset`
- Enable plugin in app.json (`["expo-asset",{"assets":["./assets/asdf.onnx"]}]`)
- Add filetype in metro.config.js (`config.resolver.assetExts.push("onnx")`)
- `npx expo prebuild --clean`

## Output
```
✔ Cleared android, ios code
› Android package name: com.developer.asdf
› Apple bundle identifier: com.developer.asdf
✔ Created native directories
✔ Updated package.json
» ios: expo-asset: `.onnx` is not a supported asset type
» android: expo-asset: `.onnx` is not a supported asset type
✔ Finished prebuild
```

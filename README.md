
# react-native-text-input-reset

## Getting started

`$ yarn add react-native-text-input-reset`

### Mostly automatic installation

`$ react-native link react-native-text-input-reset`

### Manual installation

#### Android

1. Open up `android/app/src/main/java/[...]/MainApplication.java`
  - Add `import com.nikolaiwarner.RNTextInputResetPackage;` to the imports at the top of the file
  - Add `new RNTextInputResetPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-text-input-reset'
  	project(':react-native-text-input-reset').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-text-input-reset/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-text-input-reset')
  	```

## Usage
```javascript
import TextInputReset from 'react-native-text-input-reset';

// Clear text input and keyboard suggestions
TextInputReset.resetKeyboardInput(findNodeHandle(this.textInputRef))
```

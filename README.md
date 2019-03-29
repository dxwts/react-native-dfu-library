
# react-native-dfu-library

## Getting started

`$ npm install react-native-dfu-library --save`

### Mostly automatic installation

`$ react-native link react-native-dfu-library`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-dfu-library` and add `RNDfuLibrary.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNDfuLibrary.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.onyx.dfu.RNDfuLibraryPackage;` to the imports at the top of the file
  - Add `new RNDfuLibraryPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-dfu-library'
  	project(':react-native-dfu-library').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-dfu-library/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-dfu-library')
  	```


## Usage
```javascript
import RNDfuLibrary from 'react-native-dfu-library';

// TODO: What to do with the module?
RNDfuLibrary;
```
  
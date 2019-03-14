# NativeScript-Vue Application

> A native application built with NativeScript-Vue

## Usage

<!-- ``` bash -->
# Install dependencies
`[sudo] npm install -g @vue/cli @vue/cli-init`

`vue init nativescript-vue/vue-cli-template <project name>`
`cd <project name>`

`npm install`

`tns setup`

`tns doctor (make sure everything is updated)`

`tns update (if you need to update anything)`

##Quick Fix to get Environment working 
### *(note that CocoaPods could get deprecated in the future)
`sudo gem uninstall cocoapods`<br>
  * `yes, remove executables`

`sudo gem install cocoapods -v 1.5.3`

`rm -Rf platforms`

`tns install`

`tns run <platform> --bundle`




# Build for production
`tns build <platform> --bundle`

# Build, watch for changes and debug the application
`tns debug <platform> --bundle`

# Build, watch for changes and run the application
`tns run <platform> --bundle`
```# vue-ns-env

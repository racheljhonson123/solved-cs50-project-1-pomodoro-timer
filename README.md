Download Link: https://assignmentchef.com/product/solved-cs50-project-1-pomodoro-timer
<br>
For this project, you’ll be implementing a Pomodoro timer. This timer will helppeople trying to use the [Pomodoro Technique](https://en.wikipedia.org/wiki/Pomodoro_Technique).It will vibrate to tell you when to take breaks or resume working, based on somedetermined values. Check out the [staff solution](#staff-solution) for a workingversion.

## Requirements– You may not import libraries other than the below:– `expo`– `react`– `react-native`– `prop-types`– Timer should display minutes and seconds in text– Timer should count down seconds until it reaches 00:00– Phone should buzz when timer reaches 0– Timers should switch between 25 and 5 minutes– Timer should be able to start, stop, and reset

The aesthetics of the app is up to you!

### Challenge (Not Required)– Allow the user to input any arbitrary time for the timers (e.g. 5 mins of work time and 5 mins of break)

## Getting StartedFirst, head to [this link](https://docs.expo.io/versions/latest/introduction/installation.html)to install Expo. You’ll need the XDE for your computer and the mobile client(Expo app) on your phone. If you prefer, you can also install the iOS simulator(Macs only) and/or the Android emulator.

You’ll also need Node.js and NPM installed. You can check if you already have theminstalled by opening a terminal and running `node –version` and `npm –version`.If numbers are printed, you’re good to go. If not, [install them](https://nodejs.org/en/).You’ll probably want the LTS version (v8.x.x). NPM will be installed automaticallywhen you install node.

After installing those software dependencies, you’ll need to install your app’s“dependencies” (libraries that are required to run the app, such as `react`,`react-native`, etc.). Fortunately, it’s very easy to do! From a terminal, `cd`into this directory and run the command `npm install`. NPM will look at the[`package.json`](/package.json) file’s `dependencies` key and install thoselibraries, as well as all of those libraries’ dependencies (and the dependencies’dependencies and so on).

Now you have everything installed that you need to run the app! Open the ExpoXDE app and click the `Open existing project…` button. Select the folder thatcontains this file (make sure you have the parent folder and not this file) andpress `Open`.

You should now see two panels with logs. The left will output some messeages,hopefully including `Dependency graph loaded.`. If you see this message, thenyour app is running (well technically the bundler that serves your app is running).

You can now open the app on your phone or simulator by clicking one of the buttonsin the top right. To open on your phone, click the `Share` button and scan theQR code from the Expo app on your phone. To open in a simulator, click the `Device`button and select the simulator into which you want to open your app.

When you have the app open in your phone or simulator, try opening [`App.js`](/App.js)and changing a line. You should see it update on your phone!

You can now begin to work on your app. You may find the vibrate function in[`/utils`](/utils) helpful. Feel free to import and use it in your app like this:

“`javascriptimport {vibrate} from ‘./utils’

// causes phone to vibratevibrate()“`
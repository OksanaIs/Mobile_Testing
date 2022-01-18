### Android App Design Checklist
https://developer.android.com/docs/quality-guidelines/core-app-quality

#### Navigation:
* The app must support standard back button navigation and not use back button on-screen prompts.
* The application must save the user's state when exiting and prevent accidental data loss due to back navigation.
* When resuming applications from "Recent" or after the device wakes up from sleeping (locked) state, it should return the user exactly to the state in which it was last used.

#### Notifications:
* Do not use notifications to advertise the product.
* Combine multiple notifications into one notification group.

#### User interface and graphics:
* Whenever possible, the application should support landscape and portrait orientations and minimize/restore the application window.
* The application must use the entire screen in both orientations.
* The application must quickly handle transitions between display orientation, nesting/expanding, rendering, or state loss.

#### Stability:
* The application must not crash or block the user interface.
* The app should load quickly, or provide a progress bar or any other hint if it takes more than two seconds to load.

#### Privacy and Security:
* The app must request the minimum number of permissions required to support usage. For permissions such as location, use approximate location instead of exact location if possible.
* The app should only ask for permission to access sensitive data (SMS, call log, or location) if it is related to the main use cases of the app.
* The application must clearly state the reason why certain permissions are needed.
* All sensitive data must be stored in the app's internal memory.
* The app must provide prompts for automatically completing accounts (credit card information, physical address, and phone number).
* All network traffic must be sent over SSL.

#### Support for all screen types and states:
* The app must update the user interface (keep playing videos, update new messages, update download progress, etc.).
* Modals, options menus, and other secondary elements should be well-formatted on all screen types and in all states.

#### Testing:
* If the application edits or creates content, has games, or plays media, be sure to test it.
* During testing, make interruptions from other applications, such as to receive notifications or a phone call, and apply temporary changes to the device, such as network connection, battery life, GPS availability, and system boot.
* On each app screen, press the Home key or swipe up in gesture navigation, and then re-launch the app from the All Apps screen.
* On the screen of each app, switch to another running app and then return to the app you're testing with the Recent app switcher.
* On each application screen (and dialog boxes), press the back button or use the swipe back gesture.
* On each app screen, rotate your device between landscape and portrait orientations and collapse/expand at least three times.
* Switch to another app to put the test app in the background. Go to Settings and check if the test app has any services running in the background. On Android 4.0 and later, go to the Apps screen and find the app in the Running tab.
* Press the power button to put the device to sleep, then press the power button again to turn on the screen.
* Set up a screen lock on your device. Press the power button to put the device to sleep (which locks the device). Then press the power button again to wake up the screen and unlock the device.
* Initiate and observe in the notification bar all types of notifications that the application can display. Expand notifications where applicable (Android 4.1 and up) and tap all available actions.
* Launch the app and use all the main features by watching the device log. No personal information about the user should be logged.

### iOS Human Interface Guidelines Checklist
#### https://developer.apple.com/design/human-interface-guidelines/ios/overview/themes/

#### Interface basics
Tell the app where the user is, provide navigation, add buttons or other elements to initiate actions and convey information.

#### Launching:
* Application launch process should be fast and smooth.
* Launch the application using the current device orientation. If an app only runs in one orientation, it should always run in that orientation and allow the device to be rotated as needed.
* Request settings information from device settings and defaults or via sync service (iCloud). If you need to ask for information about settings, you can provide it when you first open the application and with permission to change settings later.
* After restarting the application, save and restore the state of the application (save history).
* Let the app opt-out of rating prompts and don't force people to rate the app.

#### Loading
When downloading or updating, show an activity counter to estimate how long to wait.

#### Accessing User Data and Resources:
* Request permission to access:
    * Personal information, including location, health, financial, contact, and other personal information.
    * Emails, messages, calendar data, contacts, game information, Apple Music activities, HomeKit data, and audio, video, and photo content.
    * Bluetooth peripherals, home automation features, Wi-Fi connections, and LANs.
    * Camera, microphone.

#### Access permission request:
* Ask for permission when an app needs access to data or a resource.
* Write clear text on how the application will use the data or resource that is requested.

#### Face ID and Touch ID:
* In the app, provide a single authentication method (Face ID) and other options (requesting a username and password) as fallbacks only if the original method doesn't work.
* Name the button for signing in to the app with Face ID "Sign in with Face ID", not "Sign in".
* In an app, do not use Touch ID that supports Face ID and vice versa.

#### Data input:
* In your app, make it possible to use selectors or a table instead of a text box.
* Use the button's activation as a visual signal that it's time to act. When the required fields are filled in (activate the "Continue", "Next" button).
* Use the ability to sort lists of values ​​alphabetically or in some other logical way.
* Add placeholder text such as "Email" or "Password" to text fields when there is no other text in the field.

#### Working with files:
* Automatically save changes at regular intervals when opening and closing files and when switching to another application.
* Use Quick Look to view the contents of Keynote, Numbers, and Pages documents, PDFs, images, and more, even if the application doesn't open them.
* Provide the ability to share files with other applications.

#### Gestures:
* Use standard gestures.
* Do not use standard gestures to perform non-standard actions.
* Offer quick gestures to complement, not replace, UI-based navigation and actions.

#### Home Screen Quick Actions:
* The app must include one helpful quick action (you can provide a total of four).
* The name of the action should instantly communicate the results of the action (for example, "How to get home", "Create a new contact" and "New message").
* Do not include the app name or any extraneous information in the title or subtitle.

#### Notifications:
* Write short, easy-to-read notifications.
* Do not include sensitive, private, or confidential information in the notice.
* Avoid sending multiple notifications about the same thing even if the user didn't reply.

#### General Layout Considerations:
* Make sure users don't have to scroll horizontally to read important text, or zoom in to see key images.
* Support both portrait and landscape orientation.
* Prepare the app for text resizing.

#### Color:
* Provide text labels or glyphs so that users with color blindness or other visual impairments can understand your color to convey information.
* Provide two versions of your accent color to make sure it looks good in both light and dark modes.
* Avoid using the same color for interactive and non-interactive elements.

#### Launch screen:
* Avoid including text on the launch screen. Since the content of the launch screen does not change, any displayed text will not be localized.
* Do not add ads to the launch screen.

#### Application icon:
* Keep the background simple and avoid transparency.
* Use words only when they are necessary or are part of the logo.
* Test your icon on different wallpapers.
* Make the corners of the icons straight (the mask system automatically rounds the corners of the icons).

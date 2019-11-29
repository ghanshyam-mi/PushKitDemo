# Voice over Internet Protocol (VoIP)
In this example, I have implemeted PushKit framework for an iOS app.

Voice Over IP (VoIP) Best Practices
A Voice over Internet Protocol (VoIP) app lets the user make and receive phone calls using an Internet connection instead of the device's cellular service. Because a VoIP app relies heavily on the network, it's no surprise that making calls results in high energy use. When not in active use, however, a VoIP app should be completely idle to conserve energy

Prior to iOS 8, VoIP apps needed to maintain a persistent connection with the server to receive calls using an Internet connection. Keeping a connection open in the background, drains the battery as well as causes all kinds of problems when the app crashes or is terminated by the user.

With iOS 8 Apple introduced PushKit. PushKit improves battery life, performance and stability of messaging apps. PushKit is meant to solve these problems by offering a high-priority push notification with a large payload. The VoIP app receives the notification in the background, sets up the connection or process data and displays a local notification to the user. When the user swipes the notification, the call/data is ready to connect/display.

# There are a couple of benefits of this PushKit
	• PushKit notifications are never presented to the user - they don't present badges, alerts, or sounds.
	• Apple promises to deliver these push notifications high priority.
	• For Voice over Internet Protocol (VoIP) notifications, the maximum payload size is 5 KB (5120 bytes).
	• The device is woken only when VoIP pushes occur, saving energy.
	• VoIP pushes can include more data than what is provided with standard push notifications.
	• Your app is automatically relaunched if it's not running when a VoIP push is received.
	• Your app is given runtime to process a push, even if your app is operating in the background.


# LICENSE!
PushKitDemo is MIT-licensed.

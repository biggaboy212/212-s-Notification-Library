<h1 align="center">
  212's Notification Library
</h1>

<p align="center">
  An open-source Notification Library.
</p>

Logs: Added CreateAdminNotification, No docs because im lazy (Same arguments, but it disables all gui's including coregui's while the notification is up.) 


(!Warning! This function is new, and such is very buggy, RemoveNotifications is broken for this function, and avoid executing function multiple times before the notification is over or all of your gui's will be disabled and you will have to rejoin.)


# Documentation
### Getting loadstring
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/biggaboy212/212-s-Notification-Library/main/Source"))()
```


### Create a Notification
```lua
library:CreateNotification(5, "CenterThenBottom", "Header", "SubHeader", false, true, "Ok", 50,50,200, true, 15)
```

	1 Notification at a time. If one notification is called while another is still up, the new one will override the existing notification

	
	CreateNotification Parameters
	
	DeleteTimeout | Waits set amount, then removes the Notification | Type: Number or Bool | Inputs: false, Number
	TweenInStyle | The way the Notification comes onto your screen | Type: String | Inputs: "Bottom", "Center", "CenterThenBottom"
	HeadingText | Heading Text | Type: String | Inputs: String
	SubHeadingText | SubHeading Text | Type: String | Inputs: String
	Image | An image that will be next to your heading, use "rbxassetid://" followed by the image's asset id if you want an image. Leave false for no image | Type: Bool or String | Inputs: false or String
	ButtonEnabled | Decide if you want to have a button to close the notification manually, if false, please use DeleteTimeout to make sure the notification dosent stay forever | Type: Bool | Inputs: Bool
	ButtonText | Text for close button | Type: String | Inputs: String
	R, G, B | RGB values for the AccentBar/TopBar | Type: Number | Inputs: Number
	BlurValue | Decide if you want the screen to blur when a Notification pops up | Type: Bool | Inputs: Bool
	BlurSize | The amount that your screen will blur if blur is enabled (Default - 15) | Type: Number | Inputs: Number


### Remove Notifications
```lua
library:RemoveNotifications("Tween")
```

	RemoveNotifications Parameters
	
	RemoveType | The way that notifications will be removed | Type: String | Inputs: "Instant", "Tween"

 
### Update Notifications
```lua
library:UpdateNotifications("Updated Header", "Updated SubHeading", "rbxasset://textures/ui/GuiImagePlaceholder.png", 200,50,50)
```

	UpdateNotifications Parameters
	
	Heading | What your heading will be updated to | Type: String | Inputs: String
	SubHeading | what your SubHeading will be updated to | Type: String | Inputs: String
	Image | If image functionality wasn't initially enabled in the notification, updating with an Image ID won't add an image. Set to false if you wish to avoid updating the image for notifications with prior image enablement.



### Images

###### With button
![image](https://github.com/biggaboy212/212-s-Notification-Library/assets/75142294/07849c20-af2e-4955-bbc2-bc9fc41454c6)

###### Without button
![image](https://github.com/biggaboy212/212-s-Notification-Library/assets/75142294/b4f601cd-81be-4c7b-b14d-0249ed68af38)

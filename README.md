# 212's Notification Library

Adding real documentation later, example and testing gui is uploaded to the github

heres a very rushed documentation


# Create a Notification

	1 Notification at a time. If another notification is called while another one is still up, the new one will over-ride the existing one

	
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
Example: library:CreateNotification(5, "CenterThenBottom", "212's Notification Library", "hi :3", false, true, "Ok", 50,50,200, true, 15)


# Remove Notifications

	RemoveNotifications Parameters
	
	RemoveType | The way that notifications will be removed | Type: String | Inputs: "Instant", "Tween"
Example: library:RemoveNotifications("Tween")

 
# Update Notifications

	UpdateNotifications Parameters
	
	Heading | What your heading will be updated to | Type: String | Inputs: String
	SubHeading | what your SubHeading will be updated to | Type: String | Inputs: String
	Image | What your image will be updated to, if the notification did not already have image enabled, then it will not add an image even if you update it with an Image ID. Leave false if you do not want to update the image (if you already previously had it enabled) | Type: String | Inputs: String, false

Example: library:UpdateNotifications("update test", "updated subheading", "rbxasset://textures/ui/GuiImagePlaceholder.png", 200,50,50)


![image](https://github.com/biggaboy212/212-s-Notification-Library/assets/75142294/07849c20-af2e-4955-bbc2-bc9fc41454c6)

![image](https://github.com/biggaboy212/212-s-Notification-Library/assets/75142294/b4f601cd-81be-4c7b-b14d-0249ed68af38)

![image](https://github.com/biggaboy212/212-s-Notification-Library/assets/75142294/d14c729d-7fcb-4056-b8c2-a9e243a530ac)

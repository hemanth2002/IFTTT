# IFTTT
DIY dash button using esp 32 (or) 8266 and webhooks for IOT projects.


STEP 1:

Go to IFTTT website https://ifttt.com/explore

![IFTTT - Google Chrome 09-12-2022 13_17_00 (2)](https://user-images.githubusercontent.com/72966457/206661217-4c7959a9-1817-4807-b8e9-f0ad359153b4.png)


STEP 2:

Create a new account or login to your IFTTT account.

![New Tab - Google Chrome 09-12-2022 13_02_12 (2)](https://user-images.githubusercontent.com/72966457/206661314-45905e09-3aa0-49d9-85b8-e74dc5587db7.png)


STEP 3:

Go to create applet.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_03_28 (3)](https://user-images.githubusercontent.com/72966457/206680854-0ab64c9a-5a9c-471b-92d6-c3fef2a3aeee.png)


STEP 4:

Click "add" in 'if this'.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_03_43 (2)](https://user-images.githubusercontent.com/72966457/206661510-ced5886f-56fd-4faf-af2b-49333b881796.png)

Step 5:

Search for "Webhooks" in services.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_04_04 (2)](https://user-images.githubusercontent.com/72966457/206653204-d9c005a6-1906-4b4a-9739-ab55d40a8cd3.png)


STEP 5:

Choose the type of trigger, select "receive a web request".

![My Applets - IFTTT - Google Chrome 09-12-2022 13_04_11 (2)](https://user-images.githubusercontent.com/72966457/206661687-40fea8fe-af39-4651-ba6f-462836d228fe.png)


STEP 6:

Type the name of the trigger you want.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_05_08 (2)](https://user-images.githubusercontent.com/72966457/206654482-5849f09d-50d6-4a88-888e-ef370f1d2d3d.png)


STEP 7:

save and select "then that".

![My Applets - IFTTT - Google Chrome 09-12-2022 13_05_20 (2)](https://user-images.githubusercontent.com/72966457/206657736-a75b23be-ac94-45c2-be1d-f5520e2c63e5.png)


STEP 8:

Here you can get creative and explore the things you want to control.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_06_02 (2)](https://user-images.githubusercontent.com/72966457/206658654-ecb0e542-f17b-47c7-8eed-b5ac9a3b8469.png)

As an example, i made a smartphone to open google map to the predefined location, whenever the dashbutton is triggered (button pressed). 

Select Android phone.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_06_08 (2)](https://user-images.githubusercontent.com/72966457/206660083-8d71bb3c-96e9-4fd7-a861-a2671210b450.jpg)


STEP 9:

select google maps navigation.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_06_17 (2)](https://user-images.githubusercontent.com/72966457/206660254-af1db8ed-a42d-455c-9739-cd2c0322c31f.png)


STEP 10:

Choose the type of transport and location.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_07_12 (2)](https://user-images.githubusercontent.com/72966457/206660408-68139419-15cd-43cb-8e09-e22e5fd06ebd.png)


STEP 11:

Save and continue , meanwhile download the "IFTTT" app in your smartphone and login with the same account you logged in here. (make sure you have installed google maps already).

![My Applets - IFTTT - Google Chrome 09-12-2022 13_07_26 (2)](https://user-images.githubusercontent.com/72966457/206660834-fab16472-07b7-46e9-9919-444ab9f33d4d.png)
![My Applets - IFTTT - Google Chrome 09-12-2022 13_07_32 (2)](https://user-images.githubusercontent.com/72966457/206661012-c9c281a1-f960-4bd9-abe9-68fa3e9062ec.png)
![My Applets - IFTTT - Google Chrome 09-12-2022 13_07_42 (2)](https://user-images.githubusercontent.com/72966457/206661105-774be010-39ec-4394-8ebe-8149c503a901.png)

STEP 12:

now click on the web hook icon.

![My Applets - IFTTT - Google Chrome 09-12-2022 13_07_42 (2)](https://user-images.githubusercontent.com/72966457/206679970-6306b391-22c6-4170-8b2f-2972da3ce743.png)

STEP 13:

click documentation:

![Webhooks works better with IFTTT - Google Chrome 09-12-2022 15_55_13 (3)](https://user-images.githubusercontent.com/72966457/206681587-d06f989b-87b5-45dd-bfc0-9c8406072b6b.png)

STEP 14:

Navigate to "{event}" in the post and get web request URL.

Change the " {event} " to " button_triggered " which we previously entered in the webhook trigger command. (note: The curly brackets should also be removed and the trigger command is case sesitive and sholud be same as the one we previously entered. ) 

![IFTTT Maker Webhooks - Google Chrome 09-12-2022 15_58_09 (2)](https://user-images.githubusercontent.com/72966457/206728807-c3298956-8425-4b6f-b984-bca42d0cc90d.png)

After changing.

![IFTTT Maker Webhooks - Google Chrome 09-12-2022 20_11_50 (2)](https://user-images.githubusercontent.com/72966457/206729536-ff172ab6-3da4-493f-8d3a-f3e28d850c6f.png)

Now hit "test" and check wheather the set location open in your phone. (keep the phone unlocked and "IFTTT" app running and connected to internet).

Make sure to turn on "display over other apps" ON on your phone and turn OFF "battery saver".

STEP 15:

Now for the coding part

Type your wifi ssid, password, https URL in the code within the semicolon.

![IFTTT _ Arduino IDE 2 0 3 09-12-2022 20_48_16](https://user-images.githubusercontent.com/72966457/206734719-245b7573-e211-446a-b6ee-fb87acd35bb2.png)

Select the board type and upload.

Thats it the project is completed turn on the esp 32 or 8266 and check if works.

Everytime the reset button is pressed in the board the trigger is send and map opens everytime.
note: the IFTTT is not real time so the action can take some time depends upon the traffic. 

The whole process is mobile friendly and can be done by using your smartphone
To program the board use this app https://play.google.com/store/apps/details?id=name.antonsmirnov.android.arduinodroid2 and OTG cable to connect with the board and phone.

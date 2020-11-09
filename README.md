
# Home-automation-using-nodeMCU-ESP8266-Voice automated
Automate your home using Node MCU for SCI-tech VIIT pune (DOP = 14 March 2019 )

1>Configure the blink app by signing in and Selecting the  Node MCU ports for switiching .
https://play.google.com/store/apps/details?id=cc.blynk

2>Copy the auth token u get.

3>Download arduino blink libarary and add it in the arduino IDE.
https://github.com/blynkkk/blynk-library.git

4>Configue the arduino IDE for working with nodeMCU.

6> Open the AUTOMATION_CODE in arduino and add the auth token ,wifi SSID ,wifi key to connect with.

5>Compile and upload the AUTOMATION_CODE in nodeMCU.

6> Build and relay board for switching depending on your requirements.(you can also use pre build relay boards)

7> In our case we are using 3 mode switch which has modes
 mode_1 = turn ON
 mode_2 = dim lights (night mode)
 mode_3 = turnvOFF
 
 8> Go to IFTTT  and signin -https://ifttt.com/home
 9> create a new applet from this -https://ifttt.com/create/if-google-assistant
 10>Configure the request and response 
 11>Configure the webrequest by setting the URL  by appropriate auth token got by blink and corresponding port.(blynk app INDIA server)
 http://188.166.206.43/ YourAuthTokenHere / update / DigitalPinToBeUpdateHere
 METHOD: PUT
 CONTENT TYPE : application/json
 body : ["0"]
 
 10> And you are done . Setup  power supplies and you are ready to control your home with your voice. 

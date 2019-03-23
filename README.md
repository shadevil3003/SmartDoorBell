# SmartDoorBell
#Raspberry Pi 3 - Smart Doorbell

**Introduction:-**


Suppose you are sitting at the comforts of your room with your earphones plugged in and someone rings your doorbell , You wont know about it since you have your earphones plugged in . So to tackle this situation of carelessness we came up with a Smart Doorbell . This doorbell would send the notification to your phone whenever it detects a person near it(<20cm) along with the photo of the person. 

**Materials:-**


1)Raspberry Pi 3

2)Ultrasonic Sensor

3)Usb WebCam

4)Jumper Wires

5)BreadBoard

**Circuit:-**


Vcc - 5v

Echo - GPIO23

Trig - GPIO18

Gnd - Gnd

**Important :-**


1)**Create your own bot .** if you don't know how to create one refer to the link below:-
  https://www.instructables.com/id/Set-up-Telegram-Bot-on-Raspberry-Pi/
  
2)**Know your chat id** :- 1.Open Telegram app and search "get id" or  "@get_id_bot"

                       2.Type "/start" , You will get your chat id
                       
                       3.You can also refer to the video below :-
                         https://www.youtube.com/watch?v=2jdsvSKVXNs

**Things to change in the code :-**


1)(See Line 50 and 51) Change from the chat-id in the code to your chat-id . 
  telegram_bot.sendMessage (Chat_id, message)
  telegram_bot.sendPhoto(Chat_id,photo=open("imagetest.jpg"))
  
2)(See line 58) Change from the default_token to your token 
  telegram_bot = telepot.Bot('default_token')

**How to run .py file in Raspberry pi?**


1)Open terminal

2)Go to the .py file location

3)Type python file_name.py

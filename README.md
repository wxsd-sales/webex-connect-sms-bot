<p align="center">
  <h2 align="center">IMI Demo</h2>

  <p align="center">
    Send SMS to and from Webex spaces using a Webex bot.  Powered by Cisco's IMIMobile acquisition.
    <br />
    <a href="https://github.com/WXSD-Sales/imidemo/issues"><strong>Report Bug</strong></a>
    ·
    <a href="https://github.com/WXSD-Sales/imidemo/issues"><strong>Request Feature</strong></a>
  </p>
</p>

## About The Project

**New Video!**  
[![SMS to/from Webex Video Demo](https://img.youtube.com/vi/DGEQt4x8YLg/0.jpg)](https://youtu.be/DGEQt4x8YLg, "SMS to/from Webex")  
[Link to previous video](https://youtu.be/NY-_RQHKcsY)



### Walkthrough

To begin using the production version of this bot, **send a Webex message to imidemo@webex.bot**  
_(You can send a Webex message to a bot the same way you send a message to a person)_  

**Configuring a Team**  
1. If you have no teams configured, you should add a team first with the add team button.  
![Screen Shot 2022-02-22 at 4 47 12 PM](https://user-images.githubusercontent.com/19175490/155225388-a8eb67ea-fa91-40f5-9a96-0a4b69013b89.png)
2. You can enter any team name (i.e. your name)
3. And any US/Canadian, or Irish mobile number that is SMS enabled. (i.e. your cell/mobile number)  
_Note: a team in the bot's context is currently just a single SMS number_  

**Sending an SMS**  
1. Once a team has been configured, you can select the team from the dropdown in the card.
2. With a team selected, enter the text you want to send to the SMS number.  
![Screen Shot 2022-02-22 at 4 51 17 PM](https://user-images.githubusercontent.com/19175490/155225656-48195814-411b-4eee-b910-4651439e3c64.png)
3. Click send, and the mobile number configured as the team should receive the SMS.
4. With your mobile device, you can reply one time to the message received by your mobile device.
5. Both the sent and received messages should appear in the Webex chat with the bot.  
![Screen Shot 2022-02-22 at 4 52 31 PM](https://user-images.githubusercontent.com/19175490/155225826-090ed425-0454-417a-b5b2-1a8ed321bfac.png)

**Configuring a Custom Bot**  
This bot can be themed to look more like a given org or customer's brand.  
To get started, click the customize button of the card returned by imidemo@webex.bot. Then,
1. [Create a Webex bot](https://developer.webex.com/my-apps/new/bot).  The bot's name and icon should fit the desired look and feel.  For example, if you are creating the bot to look like a bot for a specific retail store, consider naming the bot something like, "My Retail Store Notification Bot," and using the logo of the retailer as the bot's icon.
2. Once you've created the bot, enter the bot's auth token in the corresponding card field.  
![customize](https://user-images.githubusercontent.com/19175490/155225177-10c321e7-0a4e-4824-9038-b7b9ec7fc761.png)
3. Use an image for the card header.  This can be the same image you used as the bot's logo, or a different image, but the image will need to be a public link to a .jpg or .png file.
4. Optionally, uncheck or check "Show Instructions"
5. Optionally change the name of the card header
6. Click "Add bot"

**Once you've created a custom bot, our code will automatically configure webhooks to use for your new bot.  You can then interact with the bot similar to how imidemo@webex.bot works, and use the new bot to send/receive SMS!**



## Setup

### Prerequisites & Dependencies: 
node v14.5.0  
npm 7.24.2  

npm dependencies:  
```
dotenv: ^8.2.0
express: ^4.17.1" 
got: ^11.8.3
mongodb: ^4.2.1
```


### Installation

After you clone this repo, you will need to configure a .env file (you can copy from sample.env to get started.  However, this code relies on an imiconnect flow to send and receive SMS.  Please reach out to wxsd@external.cisco.com for help configuring your own installation.  Once you've setup the .env file and imiconnect flows, you can simply:
```
npm init
npm install
npm start
```

## License
All contents are licensed under the MIT license. Please see [license](LICENSE) for details.


## Disclaimer
<!-- Keep the following here -->  
 Everything included is for demo and Proof of Concept purposes only. Use of the site is solely at your own risk. This site may contain links to third party content, which we do not warrant, endorse, or assume liability for. These demos are for Cisco Webex usecases, but are not Official Cisco Webex Branded demos.

<!-- CONTACT -->

## Contact
Please contact us at wxsd@external.cisco.com

# Discord <> Ulitma Online Bridge 
Discord & Ultima Online bridge using EasyUO. This Ultima Online Discord Bot will allow you to both send and receive messages from your Ultima online charactor using Discord chat service (Web, or mobile app). Also included is a simple vendor search. This can be combined with IFTTT.com and Google Assistant to control your Ultima Online Charactor and dictate your party/guild/general chat messages using your voice. If you use Discords tts (Text to Speech) feature, any responses in game can be read back to you in real time. Perfect for people with impaired sight, or chatting while driving. Framework can be extended easily with additional functions, and scripts. 

## Javascript Discord Bot
* discord2easyuo.js
* auth.json
* package.json

## EasyUO Scripts 
* say.euo
* journal.euo
* vendorsearch.euo

## Bash Scripts
* easyuo2discord.sh
* installduo.sh

## Bot Commands
* !say MSG - Will simply say messages outloud.
* !say \MSG - Will message in the guild chat. 
* !say /MSG - Will message in the party chat.
* !say ,MSG - Will message in the general chat.
* !vendor SEARCH ITEM - Will post a screenshot of the first page of the vendor search.
* !help - Will display this message.
* !help say - will tell more about the say.

## Dependencies
* Discord Account: [[https://discordapp.com]]
* Windows 10
* Install WSL - Windows Subsystem for Linux (Ubuntu)
  * Install here: [[https://www.microsoft.com/en-us/p/ubuntu/9nblggh4msv6]]
  * Open PowerShell as Administrator and run:
   * Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
  * Restart your computer when prompted.
* Run Ubuntu Terminal via Cortana, and create a user with same name as your windows user.
* Install git in Ubuntu terminal
  * sudo apt --yes install git #Install git without prompting

## Instructions
* Install all above dependencies ^
* Open Ubuntu terminal and run
  * cd /mnt/c/Users/$USER/Desktop/              #Change to the Desktop
  * git clone https://github.com/jphein/duo.git #Git clone the duo repository 
  * cd duo                                      #Change to the duo directory on Desktop
  * chmod u+x installduo.sh                     #Make install script executable
  * ./installduo.sh                             #Run the install script.( https://github.com/jphein/duo/blob/master/installduo.sh )
* Create Webhook for bot channel in Discord.
* Create Discord bot in @ discord.com
* Add API Token to auth.json
* (Optional) Create IFTTT.com rule to connect your Google assistant to your Discord server. For voice commands and transcription.  
* (Optional) Enable Discord TTS on bot channel. For Text to speech. Hands free chatting. 

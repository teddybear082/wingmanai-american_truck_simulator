# wingmanai-american_truck_simulator
 A config profile for American Truck Simulator for WingmanAI.

## What Is This?
This is a repo of a config I made for American Truck Simulator to use with WingmanAI by ShipBit: https://www.wingman-ai.com/.  It uses / is powered by the SCS SDK, and specifically these tools: https://github.com/RenCloud/scs-sdk-plugin and this for connecting that output to python code: https://github.com/Dreagonmon/truck_telemetry/tree/main/truck_telemetry.

Basically, it allows you to speak with three different generative artificial intelligence assistants:

(1) Assistant: Control your truck based on default keybinds.  Has web search and visionAI skills.  Has access to truck data so can answer questions about your truck, route, cargo, trailer. Can open the chat window in multiplayer and type messages automatically (“Open the chat window and type ‘Hi everyone ready to join a convoy’”).

(2) CBRadioSimulator.  Mimics talking to another random truck driver on the CBRadio using voice changer skill.  Also automatically starts simulated radio chatter between AI truckers using radio chatter skill.  To turn off say something like “turn off the CBRadio chatter.”

(3) Dispatcher.  Will have information about your truck and route.  If you say “start dispatch mode” it will check game data every ten seconds and comment on key changes, such as your new job, finished job, refueling, a fine or cargo damage.

Video here: https://www.reddit.com/r/trucksim/comments/1dr7u6e/maximum_roleplay_mode_activated/

## Quick Start

1. Download **WingmanAI**: https://www.wingman-ai.com/
2. Run the install wizard (.msi file)
3. Start the program (WingmanAI.exe) and create a free account / choose to start a free 14 day trial.
4. Close the program.
5. Navigate to **%APPDATA%/Roaming/ShipBit/WingmanAI** (your appdata is unique to your Windows user profile, so it should look something like C:\Users\{your computer user name}\AppData\Roaming\ShipBit\WingmanAI
6. Open the numbered folder, it will look something like 1_5_0 (as of this writing).  That refers to the version of Wingman.  Then click the "configs" folder.  That's where the configuration files for each game are.
7. Download the release files from this repo: https://github.com/teddybear082/wingmanai-american_truck_simulator/releases/download/wingmanai_files_1.5.0/wingmani_config_files_ats.zip.
8. Unzip those release files **directly into** the configs folder of the numbered folder above, e.g., 1_5_0/configs.  It will add a single American Truck Simulator folder to your configs folder if you did this correctly (there will not be nested folders).

![image](https://github.com/user-attachments/assets/e941be41-7e00-4ccc-bf77-f385304f0817)

![image](https://github.com/user-attachments/assets/eff062ba-8603-4608-97e1-4899479c12a3)


9. Run WingmanAI (WingmanAI.exe).  Click on the **American Truck Simulator folder** that you now see at the top of the interface, and click "Load".  Click on the Dispatcher avatar picture.  Click on the **wrench** to get to settings.  Click on **"Skills"**.  Scroll down to **ats_telemetry skill** as shown in the picture below. 
Enter the **path to your American Truck Simulator install** in the Install directory field.  **Make sure to click save** the skill setting.  Then make sure to actually **click to save again to save your profile itself**.

![image](https://github.com/teddybear082/wingmanai-american_truck_simulator/assets/87204721/6156e3f8-fad3-4fd1-ac38-4ba2fa911104)

![image](https://github.com/teddybear082/wingmanai-american_truck_simulator/assets/87204721/c7a61db2-5189-44dd-85ee-37297d65fcd9)

![image](https://github.com/teddybear082/wingmanai-american_truck_simulator/assets/87204721/4d35a4f7-45d6-4f7f-949e-db64bcd5d3eb)


11.	Start the game! You will now see a little pop up, if you didn't before, asking you to approve using advanced features.  Approve it.

12.	Once you get to the main menu, talk to your Dispatcher wingman (default: "/" key) and say "Start dispatch mode" or similar words if you want to use the simulated dispatcher feature.  The Dispatcher will confirm activation.  You can also use the configuration menu of the ats_telemetry skill to make the dispatcher automatically run without having to do this if you want.

13. Try to talk to your Wingmen! Defaults are push to talk, Delete key for CBRadioSimulator, "\\" key for Assistant and "/" key for Dispatcher.  You can also set one, like Assistant, default using the star by its name, and use "always on" voice activation mode for that one.


## What if I don't Want to Pay / Don't Want WingmanPro

The whole WingmanAI backend is open source!  You can find all the code here: https://github.com/ShipBit/wingman-ai.  You can even run it from source with python and bypass the entire .exe and UI.  Or, you can run the .exe but switch to free / local options for Speech to Text (whispercpp), LLM (choose "LocalLLM" for AI Conversation and AI Summarization Provider in the UI), and Text to Speech (You can also use EdgeTTS).

What you're likely to find, though, is that there really aren't good open source AI model options that can do function calling, which powers most of the really fun things about this project, like controlling game inputs and using the SCS SDK telemery data to get information about your game and truck.  

However, if you find a good option for local AI that can handle function calling, WingmanAI supports that!  You can change the AI provider to "LocalLLM" in the user interface and tell WingmanAI where to find it.

If, like me, you can't find a good local AI provider, you can also try Groq, which is a free LLM provider using Llama3/Llama3.1.  The only problem is we don't know how long Groq will be free and it is rate limited. You'll need a Groq API key.

The truth is, WingmanAI can be customized extensively, and it's too detailed a subject to cover in this readme.  Hop on their discord and there are plenty of folks willing to help out!  Discord link: https://discord.gg/k8tTBar3gZ


## What do you get out of this?

Nothing really, I think WingmanAI is just a super fun project and want to help people use it with their games.  Because of my early use of WingmanAI showing off a lot of custom stuff, I was invited to be a volunteer mod on their discord.  For doing that, I get a free WingmanPro sub for myself.  I don't get any sort of referral commissions or pay or anything like that.  I also contribute open-source code to the repo when I can be helpful.

## How Do I Support You If I Like This Alot?

I don't need anything! If you have a few bucks, use it to keep up a Wingman Pro sub, or buy another DLC :)!

## I'm Having a Problem With Using This

Join the wingmanai discord and find me, I'm happy to help! https://discord.gg/k8tTBar3gZ.  You can also post issues on this github.

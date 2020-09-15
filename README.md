# Age of Empires 2 DE: AI-League
Hello!

I would like to introduce you to over a month of my work. I simulated 1190 games (35 civilizations - round-robin * 2). Extreme AI vs Extreme AI on Arabia. 

The simulation itself lasted over a week, with the computer turned on all day and night. During the simulation, [my program - AutomationBoot](https://github.com/Patresss/AutomationBoot) took screens with statistics after each game.

Then I started to analyze the data. Unfortunately, [my OCR program](https://github.com/Patresss/Age-of-Empires---Stats-OCR) was not always 100% accurate, so I had to verify the values after conversion. 
1190 games * 27 columns * 2 players = 64260 values... This was definitely the most monotonous part of my project. I was partly able to introduce automatic data verification (e.g. military + economy + technology + society = total score), but this was not always possible.

If you like the project, you can [buy me a beer](https://www.buymeacoffee.com/Patres). 

Enjoy!

## Results

![](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/Result/Result.png?raw=true)

### Table
![](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/Result/Age%20of%20Empires%202%20DE_%20AI%20League%20-%20Table.png?raw=true)

### Counter civilizations
In this case, every civilization has fought every civilization only twice, so I would not take this table too seriously.
![](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/Result/Age%20of%20Empires%202%20DE_%20AI%20League%20-%20Counter%20civilizations.png?raw=true)

### Data

The data comes from [Google Sheet](https://docs.google.com/spreadsheets/d/1_R7zGNS204BG7fmou_NrhmuBG8hgbKvRfOtMSqqWfps/edit?usp=sharing)

You can also view all games in the "Games" tab.

**Please note**: As I mentioned, my OCR was not 100% correct and I verified the data manually. However, I am sure I overlooked some of the errors. If you find any result suspicious or you find an error, please let me know. Thanks!

All images can be found here: [Images](Games.md)

## Technical details
### Simulations

To simulate games, I used my application - [AutomationBoot](https://github.com/Patresss/AutomationBoot). The program clicked itself, creating new games and taking screenshoots.
* [AOE2 - AI - main.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20main.ab)
* [AOE2 - AI - fight.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20fight.ab)
* [AOE2 - AI - fight and end.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20fight%20and%20end.ab)
* [AOE2 - AI - Play.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20Play.ab)
* [AOE2 - AI - Play - Player1.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20Play%20-%20Player1.ab)
* [AOE2 - AI - Select.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20Select.ab)
* [AOE2 - AI - start.ab](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/Scripts/AOE2%20-%20AI%20-%20start.ab)

Example of the script: 

![](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/blob/master/AutomationBoot/AOE2%20-%20AI%20-%20fight%20and%20end.png?raw=true)


If you want to do this:
* Download [the scripts](https://github.com/Patresss/Age-of-Empires-2-DE---AI-League/tree/master/AutomationBoot/Scripts)
* Replace `P:\Programowanie\Projekty\AutomationBoot\MyExamples\AOE\` to your directory with the files
* Run them using [AutomationBoot](https://github.com/Patresss/AutomationBoot)

Importantly, before starting the simulation, you should set "save an uncompressed copy" on Steam so that OCR can better convert the image to text. Unfortunately I did not do it right away, so there are only games from Koreans in the Uncompressed folder.

## OCR - images into text
I described the conversion in my separate project - [Age of Empires - Stats OCR](https://github.com/Patresss/Age-of-Empires---Stats-OCR)

## Data analysis
Google Sheet was used for data analysis - [Google Sheet](https://docs.google.com/spreadsheets/d/1_R7zGNS204BG7fmou_NrhmuBG8hgbKvRfOtMSqqWfps/edit?usp=sharing)
* Copied the data to the sheet and created checksums to detect potential errors from OCR
* Calculated averages for all civilizations.
* Created tables with Counter civilizations

## If you like the project, you can donate me - thanks!

* [Buy me a coffee](https://www.buymeacoffee.com/Patres)
* [Paypal](https://www.paypal.me/Patresssss)



# C# Splatnet2 Rich Presence
#### For all your discord needs!

## Requirements
To use this program you have to have:
- .Net core and .NET framwork 4.6+ (Please make sure its **runtime** unless you want to develop with C#, you can get them [here](https://www.microsoft.com/net/download).
- Your Splatnet cookie, go [here](https://github.com/frozenpandaman/splatnet2statink/wiki/mitmproxy-instructions) to find out how to obtain it.
- All DLL's included with the repository, has to be in the same folder as the application.
- Internet connection and discord.

## Setup
1. Make sure you have .NET framework 4.6+ **runtime** and .NET Core **runtime**.
2. Open discord.
3. Run this program, input your cookie, and it will start displaying results of last match.

## Changelog 12/3/18
- Salmon run is now implemented into the RPC
- Modes used to specify what RPC you want
- No longer using C# discord wrapper because it crashes, now using the official discord-rpc dll
- Using the dll means no more errors when the user closes discord
- Statuses now appear when using the program, just to inform the user.
- Self determining Mode for both battles and salmon.

## Changelog 10/23/18
- New icon, useless but its there.
- Program notifies you if you dont have internet, which you should.
- Ability to set how long it takes to get new results, a neat thing thats changeable.
- Nerdy code stuff down below :point_down:
- Thread is no longer put to sleep, instead methods are using task.delay() so that other methods run at the same time.
- Writing to config is much easier now, grabs everything from config and splits it into a string array the array is cleaned and then checked to see if existing values exist, of they do then overrite it, if not create a new file, then write everything to lines.
- Timer added to with user's inputted time, every elapse a new json is pulled.
- Removing as many break;'s as possible because its not good.
- The Interval being inputted in console will make the user redo the input if it is not an int.

## Questions? Answers.

##### Whats this automatic mode?
This new mode can determine your most recent game for you! It will either display your salmon run results or Battles results depending on what you played last

##### This isnt my current game? why cant it show my current game?
The splatnet API does not give us the current game, only the last game played.

##### What is config.txt?
This is where your cookie and other things are stored. Keep it safe because if someone gets a hold of your cookie they can easily get your results, which isnt fine.

## Known issues
- Without the Newtonsoft.Json.dll the program wont even run, this is C#'s fault.
- Any other errors please create an issue on this repository.

## Credits
Thank you to the Discord team for the Discord RPC DLL

## Thanks
Thanks to @Valerokai for inspiration of a RPC!
Thanks to @frozenpandaman for mitmproxy instructions and inspiration for splatnet related things!
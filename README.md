# C# Splatnet2 Rich Presence
#### For all your discord needs!

## Requirements
To use this program you have to have:
- .Net core and .NET framwork 4.6+ (Please make sure its **runtime** unless you want to develop with C#, you can get them [here](https://www.microsoft.com/net/download).
- Your Splatnet cookie, go [here](https://github.com/frozenpandaman/splatnet2statink/wiki/mitmproxy-instructions) to find out how to obtain it.
- Internet connection and discord.

## Setup
1. Make sure you have .NET framework 4.6+ **runtime** and .NET Core **runtime**.
2. Open discord.
3. Run this program and it will start displaying results of last match.
 
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

##### This isnt my current game? why cant it show my current game?
The splatnet API does not give us the current game, only the last game played.

##### What is config.txt?
This is where your cookie and other things are stored. Keep it safe because if someone gets a hold of your cookie they can easily get your results, which isnt fine.

## Known issues
- Closing discord while the program is running will lead to an unstopable error, which will instantly kill the program.
- Any other errors please create an issue on this repository.

## Credits
<<<<<<< HEAD
Thank you to @Lachee for providing the discord RPC C# wrapper
=======
Thanks to Lachee for the C# RPC wrapper
>>>>>>> 4caffc00210380dec0f86c956ab180d0dbb0ad28

## Thanks
Thanks to @Valerokai for inspiration of a RPC!
Thanks to @frozenpandaman for mitmproxy instructions and inspiration for splatnet related things!
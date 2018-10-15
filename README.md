# C# Splatnet2 Rich Presence
#### For all your discord needs!

## Requirements
To use this program you have to have:
- .Net core and .NET framwork 4.6+ (Please make sure its **runtime** unless you want to develop with C#, you can get them [here](https://www.microsoft.com/net/download).
- Your Splatnet cookie, go [here](https://github.com/frozenpandaman/splatnet2statink/wiki/mitmproxy-instructions) to find out how to obtain it.
- Internet connection and discord.

## Setup
1. Make sure you have .NET framework 4.6+ **runtime**and .NET Core **runtime**.
2. Open discord.
3. Run this program and it will start displaying results of last match.
 
## Questions? Answers.

##### This isnt my current game? why cant it show my current game?
The splatnet API does not give us the current game, only the last game played.

##### What is config.txt?
This is where your cookie is stored. Keep it safe because if someone gets a hold of your cookie they can easily get your results, which isnt fine.

## Known issues
- Closing discord while the program is running will lead to an unstopable error, which requires the program to restart manually
- Without internet the program will say incorrect cookie no matter what even when cookie is correct
- Any other errors please create an issue on this repository.

## Thanks
Thanks to @Valerokai for inspiration of a RPC!
Thanks to @frozenpandaman for mitmproxy instructions and more inspiration!
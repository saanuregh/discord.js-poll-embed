<div align="center">
  <p>
    <a href="https://nodei.co/npm/discord.js-poll-embed
/"><img src="https://nodei.co/npm/discord.js-poll-embed.png?downloads=true&stars=true" alt="NPM info" /></a>
  </p>
</div>


# discord.js-poll-embed
A simple utility to create polls with just embeds and emoji reactions. No poll API required, just Discord.js reactions. By default supports following functionalities,
* By default supports 10 poll options (can be increased).
* Timed poll.
* Force closing poll.
* Custom emojis for voting (Required for bypassing default options limit)

Supports only discord.js@^12.0.0 (master).
# Installation
* `npm install discord.js-poll-embed`

# Usage
__Basic Bot Example__
```js
// Import the discord.js-pagination package
const pollEmbed = require('discord.js-poll-embed');

// Call the pollEmbed method, first three arguments are required
// title is the poll title
// options is an array of strings, which contains the poll options
// timeout is the time in seconds for which users can vote for. 0 makes it infinite and default value is 30 seconds
// emojiList is the list of emojis used for voting. Defaults to 10 simple digit emojis. Which also limits the no of options you can give by default to 10. While using custom emojis be careful that discord doesnt support some emojis.
// forceEndPollEmoji is the emoji which can be voted by the poll author to force close voting. Default value is a green check box.
pollEmbed(msg, title, options, timeout, emojiList, forceEndPollEmoji);
// There you go, now you have poll embeds
```
# Preview
![Demo](https://raw.githubusercontent.com/saanuregh/discord.js-poll-embed/master/demo.png)  
Here is a preview.

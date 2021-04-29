# A basic and easy to use discord chatbot module!

# Features

- Easy to use
- Beginner friendly
- Fast
- Works with any discord.js version!

# Example code:

```javascript
const Discord = require("discord.js");
const client = new Discord.Client();
const Chat = require("discord.chatbot");
const chat = new Chat({ name: "your bot name" });

client.on("ready", () => {
  console.log(`Ready! Logged in as ${client.user.tag}!`);
});

client.on("message", async message => {
  let reply = await chat.chat(message.content);
  message.channel.send(reply);
});

client.login("Your Token Here");
```

<br>

# Constructor options.

```javascript
const Chat = require("discord.chatbot");
const chat = new Chat({ name: "your bot name" });
```

- name: sets the name of the chatbot to provided name. By default the name is "ChatBot"

<br>

# Note:

- If you are facing any type of bugs while using this package, report them [here](https://github.com/TheLastGamer18/discord.chatbot/issues).

<br>

# Want to contribute? Feel free to make a pull request [here](https://github.com/TheLastGamer18/discord.chatbot/) and I will be happy to review it.

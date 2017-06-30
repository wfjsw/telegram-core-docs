# replyKeyboardHide

Upon receiving a message with this object, Telegram clients will remove the current custom keyboard and display the default letter-keyboard. By default, custom keyboards are displayed until a new keyboard is sent by a bot. An exception is made for one-time keyboards that are hidden immediately after the user presses a button.

<pre>
<a href="../constructor/replyKeyboardHide.md">replyKeyboardHide</a>#a03e5b85 flags:# selective:flags.2?<a href="../type/true.md">true</a> = <a href="../type/ReplyMarkup.md">ReplyMarkup</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Param description |
| **selective** | flags.2?<a href="../type/true.md">true</a> | Optional. Use this parameter if you want to remove the keyboard for specific users only. Targets: 1) users that are @mentioned in the text of the Message object; 2) if the bot's message is a reply, sender of the original message. |

## Type

<a href="../type/ReplyMarkup.md">ReplyMarkup</a>

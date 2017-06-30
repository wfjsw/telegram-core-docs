# replyKeyboardForceReply

Upon receiving a message with this object, Telegram clients will display a reply interface to the user (act as if the user has selected the bot‘s message and tapped &#39;Reply&#39;).

<pre>
<a href="../constructor/replyKeyboardForceReply.md">replyKeyboardForceReply</a>#f4108aa0 flags:# single_use:flags.1?<a href="../type/true.md">true</a> selective:flags.2?<a href="../type/true.md">true</a> = <a href="../type/ReplyMarkup.md">ReplyMarkup</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Param description |
| **single_use** | flags.1?<a href="../type/true.md">true</a> | Param description |
| **selective** | flags.2?<a href="../type/true.md">true</a> | Optional. Use this parameter if you want to force reply from specific users only. Targets: 1) users that are @mentioned in the text of the Message object; 2) if the bot's message is a reply, sender of the original message. |

## Type

<a href="../type/ReplyMarkup.md">ReplyMarkup</a>

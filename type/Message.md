# Message

Object describing a message.

<pre>
<a href="../constructor/messageEmpty.md">messageEmpty</a>#83e5de54 id:<a href="../type/int.md">int</a> = <a href="../type/Message.md">Message</a>;
<a href="../constructor/message.md">message</a>#c09be45f flags:# out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> post:flags.14?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> from_id:flags.8?<a href="../type/int.md">int</a> to_id:<a href="../type/Peer.md">Peer</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> media:flags.9?<a href="../type/MessageMedia.md">MessageMedia</a> reply_markup:flags.6?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; views:flags.10?<a href="../type/int.md">int</a> edit_date:flags.15?<a href="../type/int.md">int</a> = <a href="../type/Message.md">Message</a>;
<a href="../constructor/messageService.md">messageService</a>#9e19a1f6 flags:# out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> post:flags.14?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> from_id:flags.8?<a href="../type/int.md">int</a> to_id:<a href="../type/Peer.md">Peer</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> action:<a href="../type/MessageAction.md">MessageAction</a> = <a href="../type/Message.md">Message</a>;

</pre>

## Constructors

| Name | Description |
|------|-------------|
| [messageEmpty](../constructor/messageEmpty.md) | Empty constructor, non-existent message. |
| [message](../constructor/message.md) | Message |
| [messageService](../constructor/messageService.md) | Service message. |


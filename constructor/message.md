# message

Message

<pre>
<a href="../constructor/message.md">message</a>#c09be45f flags:# out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> post:flags.14?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> from_id:flags.8?<a href="../type/int.md">int</a> to_id:<a href="../type/Peer.md">Peer</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> media:flags.9?<a href="../type/MessageMedia.md">MessageMedia</a> reply_markup:flags.6?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; views:flags.10?<a href="../type/int.md">int</a> edit_date:flags.15?<a href="../type/int.md">int</a> = <a href="../type/Message.md">Message</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Flag mask for the message:<br> `flags & 0x1` - message is unread (moved here from **unread**)<br> `flags & 0x2` - message was sent by the current user (moved here from **out**)<br> Parameter was added in Layer 17. |
| **out** | flags.1?<a href="../type/true.md">true</a> | If true, message was sent by the current user<br> Parameter deprecated as of Layer 17. |
| **mentioned** | flags.4?<a href="../type/true.md">true</a> | Param description |
| **media_unread** | flags.5?<a href="../type/true.md">true</a> | Param description |
| **silent** | flags.13?<a href="../type/true.md">true</a> | Param description |
| **post** | flags.14?<a href="../type/true.md">true</a> | Param description |
| **id** | <a href="../type/int.md">int</a> | Message id |
| **from_id** | flags.8?<a href="../type/int.md">int</a> | Message sender |
| **to_id** | <a href="../type/Peer.md">Peer</a> | Message recipient |
| **fwd_from** | flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> | Param description |
| **via_bot_id** | flags.11?<a href="../type/int.md">int</a> | Param description |
| **reply_to_msg_id** | flags.3?<a href="../type/int.md">int</a> | Param description |
| **date** | <a href="../type/int.md">int</a> | Date created |
| **message** | <a href="../type/string.md">string</a> | Message text |
| **media** | flags.9?<a href="../type/MessageMedia.md">MessageMedia</a> | Media content |
| **reply_markup** | flags.6?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> | Param description |
| **entities** | flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; | Param description |
| **views** | flags.10?<a href="../type/int.md">int</a> | Param description |
| **edit_date** | flags.15?<a href="../type/int.md">int</a> | Param description |

## Type

<a href="../type/Message.md">Message</a>

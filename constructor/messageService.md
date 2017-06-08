# messageService

Service message.

<pre>
<a href="../constructor/messageService.md">messageService</a>#9e19a1f6 flags:# out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> post:flags.14?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> from_id:flags.8?<a href="../type/int.md">int</a> to_id:<a href="../type/Peer.md">Peer</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> action:<a href="../type/MessageAction.md">MessageAction</a> = <a href="../type/Message.md">Message</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Flag mask for the message:<br> `flags & 0x1` - message is unread (moved here from **unread**)<br> `flags & 0x2` - message was sent by the current user (moved here from **out**)<br> Parameter was added in Layer 17. |
| **out** | flags.1?<a href="../type/true.md">true</a> | Whether the message was sent by the current user<br> Parameter is deprecated since Layer 17. |
| **mentioned** | flags.4?<a href="../type/true.md">true</a> | Param description |
| **media_unread** | flags.5?<a href="../type/true.md">true</a> | Param description |
| **silent** | flags.13?<a href="../type/true.md">true</a> | Param description |
| **post** | flags.14?<a href="../type/true.md">true</a> | Param description |
| **id** | <a href="../type/int.md">int</a> | Message identifier |
| **from_id** | flags.8?<a href="../type/int.md">int</a> | Message sender |
| **to_id** | <a href="../type/Peer.md">Peer</a> | Message recipient |
| **reply_to_msg_id** | flags.3?<a href="../type/int.md">int</a> | Param description |
| **date** | <a href="../type/int.md">int</a> | Date created |
| **action** | <a href="../type/MessageAction.md">MessageAction</a> | Param description |

## Type

<a href="../type/Message.md">Message</a>

# messages.forwardMessages

Forwards messages by their IDs.

<pre>
<a href="../constructor/updatesTooLong.md">updatesTooLong</a>#e317af7e = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortMessage.md">updateShortMessage</a>#914fbf11 flags:# out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> user_id:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortChatMessage.md">updateShortChatMessage</a>#16812688 flags:# out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> from_id:<a href="../type/int.md">int</a> chat_id:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShort.md">updateShort</a>#78d4dec1 update:<a href="../type/Update.md">Update</a> date:<a href="../type/int.md">int</a> = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updatesCombined.md">updatesCombined</a>#725b04c3 updates:Vector&lt;<a href="../type/Update.md">Update</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; date:<a href="../type/int.md">int</a> seq_start:<a href="../type/int.md">int</a> seq:<a href="../type/int.md">int</a> = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updates.md">updates</a>#74ae4240 updates:Vector&lt;<a href="../type/Update.md">Update</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; date:<a href="../type/int.md">int</a> seq:<a href="../type/int.md">int</a> = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortSentMessage.md">updateShortSentMessage</a>#11f1331c flags:# out:flags.1?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> media:flags.9?<a href="../type/MessageMedia.md">MessageMedia</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;

---functions---
<a href="../method/messages.forwardMessages.md">messages.forwardMessages</a>#708e0195 flags:# silent:flags.5?<a href="../type/true.md">true</a> background:flags.6?<a href="../type/true.md">true</a> with_my_score:flags.8?<a href="../type/true.md">true</a> from_peer:<a href="../type/InputPeer.md">InputPeer</a> id:Vector&lt;<a href="../type/int.md">int</a>&gt; random_id:Vector&lt;<a href="../type/long.md">long</a>&gt; to_peer:<a href="../type/InputPeer.md">InputPeer</a> = <a href="../type/Updates.md">Updates</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Param description |
| **silent** | flags.5?<a href="../type/true.md">true</a> | Prevent the message from producing a sound notification |
| **background** | flags.6?<a href="../type/true.md">true</a> | Param description |
| **with_my_score** | flags.8?<a href="../type/true.md">true</a> | Param description |
| **from_peer** | <a href="../type/InputPeer.md">InputPeer</a> | User or chat where messages are occupied |
| **id** | Vector&lt;<a href="../type/int.md">int</a>&gt; | Message ID list |
| **random_id** | Vector&lt;<a href="../type/long.md">long</a>&gt; | Unique client message ID required to prevent message resending |
| **to_peer** | <a href="../type/InputPeer.md">InputPeer</a> | User or chat where messages will be forwarded |

## Result

<a href="../type/Updates.md">Updates</a>


# messages.sendMessage

Sends a text message.

<pre>
<a href="../constructor/updatesTooLong.md">updatesTooLong</a>#e317af7e = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortMessage.md">updateShortMessage</a>#914fbf11 flags:<a href="../type/#.md">#</a> out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> user_id:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortChatMessage.md">updateShortChatMessage</a>#16812688 flags:<a href="../type/#.md">#</a> out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> from_id:<a href="../type/int.md">int</a> chat_id:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShort.md">updateShort</a>#78d4dec1 update:<a href="../type/Update.md">Update</a> date:<a href="../type/int.md">int</a> = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updatesCombined.md">updatesCombined</a>#725b04c3 updates:Vector&lt;<a href="../type/Update.md">Update</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; date:<a href="../type/int.md">int</a> seq_start:<a href="../type/int.md">int</a> seq:<a href="../type/int.md">int</a> = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updates.md">updates</a>#74ae4240 updates:Vector&lt;<a href="../type/Update.md">Update</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; date:<a href="../type/int.md">int</a> seq:<a href="../type/int.md">int</a> = <a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortSentMessage.md">updateShortSentMessage</a>#11f1331c flags:<a href="../type/#.md">#</a> out:flags.1?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> date:<a href="../type/int.md">int</a> media:flags.9?<a href="../type/MessageMedia.md">MessageMedia</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;

---functions---
<a href="../method/messages.sendMessage.md">messages.sendMessage</a>#fa88427a flags:<a href="../type/#.md">#</a> no_webpage:flags.1?<a href="../type/true.md">true</a> silent:flags.5?<a href="../type/true.md">true</a> background:flags.6?<a href="../type/true.md">true</a> clear_draft:flags.7?<a href="../type/true.md">true</a> peer:<a href="../type/InputPeer.md">InputPeer</a> reply_to_msg_id:flags.0?<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> random_id:<a href="../type/long.md">long</a> reply_markup:flags.2?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.3?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = <a href="../type/Updates.md">Updates</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | <a href="../type/#.md">#</a> | Param description |
| **no_webpage** | flags.1?<a href="../type/true.md">true</a> | Disables link previews for links in this message |
| **silent** | flags.5?<a href="../type/true.md">true</a> | Prevent the message from producing a sound notification |
| **background** | flags.6?<a href="../type/true.md">true</a> | Param description |
| **clear_draft** | flags.7?<a href="../type/true.md">true</a> | Whether clear the draft after message sent |
| **peer** | <a href="../type/InputPeer.md">InputPeer</a> | User or chat where a message will be sent |
| **reply_to_msg_id** | flags.0?<a href="../type/int.md">int</a> | Param description |
| **message** | <a href="../type/string.md">string</a> | Message text |
| **random_id** | <a href="../type/long.md">long</a> | Unique client message ID required to prevent message resending |
| **reply_markup** | flags.2?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> | Additional interface options. A constructor for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user. (for bots only) |
| **entities** | flags.3?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; | Special entities that appear in message, such as usernames, URLs, bot commands, etc. |

## Result

<a href="../type/Updates.md">Updates</a>

## Possible errors

| Code | Type | Description |
|------|------|-------------|
| **400 BAD_REQUEST** | PEER_ID_INVALID | Invalid peer |
| **400 BAD_REQUEST** | MESSAGE_EMPTY | Empty or invalid UTF8 message was sent |
| **400 BAD_REQUEST** | MESSAGE_TOO_LONG | Message was too long.<br> Current maximum length is 4096 UTF8 characters |

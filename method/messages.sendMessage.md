# messages.sendMessage

Sample Description

<pre>
<a href="../constructor/updatesTooLong">updatesTooLong</a>#e317af7e = undefined<a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortMessage">updateShortMessage</a>#914fbf11 flags:undefined<a href="../type/#.md">#</a> out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> id:undefined<a href="../type/int.md">int</a> user_id:undefined<a href="../type/int.md">int</a> message:undefined<a href="../type/string.md">string</a> pts:undefined<a href="../type/int.md">int</a> pts_count:undefined<a href="../type/int.md">int</a> date:undefined<a href="../type/int.md">int</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = undefined<a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortChatMessage">updateShortChatMessage</a>#16812688 flags:undefined<a href="../type/#.md">#</a> out:flags.1?<a href="../type/true.md">true</a> mentioned:flags.4?<a href="../type/true.md">true</a> media_unread:flags.5?<a href="../type/true.md">true</a> silent:flags.13?<a href="../type/true.md">true</a> id:undefined<a href="../type/int.md">int</a> from_id:undefined<a href="../type/int.md">int</a> chat_id:undefined<a href="../type/int.md">int</a> message:undefined<a href="../type/string.md">string</a> pts:undefined<a href="../type/int.md">int</a> pts_count:undefined<a href="../type/int.md">int</a> date:undefined<a href="../type/int.md">int</a> fwd_from:flags.2?<a href="../type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="../type/int.md">int</a> reply_to_msg_id:flags.3?<a href="../type/int.md">int</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = undefined<a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShort">updateShort</a>#78d4dec1 update:undefined<a href="../type/Update.md">Update</a> date:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updatesCombined">updatesCombined</a>#725b04c3 updates:undefinedVector&lt;<a href="../type/Update.md">Update</a>&gt; users:undefinedVector&lt;<a href="../type/User.md">User</a>&gt; chats:undefinedVector&lt;<a href="../type/Chat.md">Chat</a>&gt; date:undefined<a href="../type/int.md">int</a> seq_start:undefined<a href="../type/int.md">int</a> seq:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updates">updates</a>#74ae4240 updates:undefinedVector&lt;<a href="../type/Update.md">Update</a>&gt; users:undefinedVector&lt;<a href="../type/User.md">User</a>&gt; chats:undefinedVector&lt;<a href="../type/Chat.md">Chat</a>&gt; date:undefined<a href="../type/int.md">int</a> seq:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Updates.md">Updates</a>;
<a href="../constructor/updateShortSentMessage">updateShortSentMessage</a>#11f1331c flags:undefined<a href="../type/#.md">#</a> out:flags.1?<a href="../type/true.md">true</a> id:undefined<a href="../type/int.md">int</a> pts:undefined<a href="../type/int.md">int</a> pts_count:undefined<a href="../type/int.md">int</a> date:undefined<a href="../type/int.md">int</a> media:flags.9?<a href="../type/MessageMedia.md">MessageMedia</a> entities:flags.7?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = undefined<a href="../type/Updates.md">Updates</a>;

---functions---
<a href="../method/messages.sendMessage.md">messages.sendMessage</a>#fa88427a flags:undefined<a href="../type/#.md">#</a> no_webpage:flags.1?<a href="../type/true.md">true</a> silent:flags.5?<a href="../type/true.md">true</a> background:flags.6?<a href="../type/true.md">true</a> clear_draft:flags.7?<a href="../type/true.md">true</a> peer:undefined<a href="../type/InputPeer.md">InputPeer</a> reply_to_msg_id:flags.0?<a href="../type/int.md">int</a> message:undefined<a href="../type/string.md">string</a> random_id:undefined<a href="../type/long.md">long</a> reply_markup:flags.2?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.3?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = undefined<a href="../type/Updates.md">Updates</a>;
</pre>

## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | undefined&lt;a href=&#34;../type/#.md&#34;&gt;#&lt;/a&gt; | Param description |
| **no_webpage** | flags.1?&lt;a href=&#34;../type/true.md&#34;&gt;true&lt;/a&gt; | Param description |
| **silent** | flags.5?&lt;a href=&#34;../type/true.md&#34;&gt;true&lt;/a&gt; | Param description |
| **background** | flags.6?&lt;a href=&#34;../type/true.md&#34;&gt;true&lt;/a&gt; | Param description |
| **clear_draft** | flags.7?&lt;a href=&#34;../type/true.md&#34;&gt;true&lt;/a&gt; | Param description |
| **peer** | undefined&lt;a href=&#34;../type/InputPeer.md&#34;&gt;InputPeer&lt;/a&gt; | Param description |
| **reply_to_msg_id** | flags.0?&lt;a href=&#34;../type/int.md&#34;&gt;int&lt;/a&gt; | Param description |
| **message** | undefined&lt;a href=&#34;../type/string.md&#34;&gt;string&lt;/a&gt; | Param description |
| **random_id** | undefined&lt;a href=&#34;../type/long.md&#34;&gt;long&lt;/a&gt; | Param description |
| **reply_markup** | flags.2?&lt;a href=&#34;../type/ReplyMarkup.md&#34;&gt;ReplyMarkup&lt;/a&gt; | Param description |
| **entities** | flags.3?Vector&amp;lt;&lt;a href=&#34;../type/MessageEntity.md&#34;&gt;MessageEntity&lt;/a&gt;&amp;gt; | Param description |

## Result

Returns undefined&lt;a href=&#34;../type/Updates.md&#34;&gt;Updates&lt;/a&gt;

Describe the result


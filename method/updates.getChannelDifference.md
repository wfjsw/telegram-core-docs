# updates.getChannelDifference

Sample Description

<pre>
<a href="../constructor/updates.channelDifferenceEmpty">updates.channelDifferenceEmpty</a>#3e11affb flags:<a href="../type/#.md">#</a> final:<a href="../type/flags.0?true.md">flags.0?true</a> pts:<a href="../type/int.md">int</a> timeout:<a href="../type/flags.1?int.md">flags.1?int</a> = <a href="../type/updates.ChannelDifference.md">updates.ChannelDifference</a>;
<a href="../constructor/updates.channelDifferenceTooLong">updates.channelDifferenceTooLong</a>#410dee07 flags:<a href="../type/#.md">#</a> final:<a href="../type/flags.0?true.md">flags.0?true</a> pts:<a href="../type/int.md">int</a> timeout:<a href="../type/flags.1?int.md">flags.1?int</a> top_message:<a href="../type/int.md">int</a> read_inbox_max_id:<a href="../type/int.md">int</a> read_outbox_max_id:<a href="../type/int.md">int</a> unread_count:<a href="../type/int.md">int</a> messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/updates.ChannelDifference.md">updates.ChannelDifference</a>;
<a href="../constructor/updates.channelDifference">updates.channelDifference</a>#2064674e flags:<a href="../type/#.md">#</a> final:<a href="../type/flags.0?true.md">flags.0?true</a> pts:<a href="../type/int.md">int</a> timeout:<a href="../type/flags.1?int.md">flags.1?int</a> new_messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; other_updates:Vector&lt;<a href="../type/Update.md">Update</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/updates.ChannelDifference.md">updates.ChannelDifference</a>;

---functions---
<a href="../method/updates.getChannelDifference.md">updates.getChannelDifference</a>#3173d78 flags:<a href="../type/#.md">#</a> force:<a href="../type/flags.0?true.md">flags.0?true</a> channel:<a href="../type/InputChannel.md">InputChannel</a> filter:<a href="../type/ChannelMessagesFilter.md">ChannelMessagesFilter</a> pts:<a href="../type/int.md">int</a> limit:<a href="../type/int.md">int</a> = <a href="../type/updates.ChannelDifference.md">updates.ChannelDifference</a>;
</pre>

## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | [#](../type/#.md) | Param description |
| **force** | [flags.0?true](../type/flags.0?true.md) | Param description |
| **channel** | [InputChannel](../type/InputChannel.md) | Param description |
| **filter** | [ChannelMessagesFilter](../type/ChannelMessagesFilter.md) | Param description |
| **pts** | [int](../type/int.md) | Param description |
| **limit** | [int](../type/int.md) | Param description |

## Result

Describe the result


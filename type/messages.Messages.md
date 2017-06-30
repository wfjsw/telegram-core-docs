# messages.Messages

Sample Description

<pre>
<a href="../constructor/messages.messages.md">messages.messages</a>#8c718e87 messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/messages.Messages.md">messages.Messages</a>;
<a href="../constructor/messages.messagesSlice.md">messages.messagesSlice</a>#b446ae3 count:<a href="../type/int.md">int</a> messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/messages.Messages.md">messages.Messages</a>;
<a href="../constructor/messages.channelMessages.md">messages.channelMessages</a>#99262e37 flags:# pts:<a href="../type/int.md">int</a> count:<a href="../type/int.md">int</a> messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/messages.Messages.md">messages.Messages</a>;

---functions---
<a href="../method/messages.getMessages.md">messages.getMessages</a>#4222fa74 id:Vector&lt;<a href="../type/int.md">int</a>&gt; = <a href="../type/messages.Messages.md">messages.Messages</a>;
<a href="../method/messages.getHistory.md">messages.getHistory</a>#afa92846 peer:<a href="../type/InputPeer.md">InputPeer</a> offset_id:<a href="../type/int.md">int</a> offset_date:<a href="../type/int.md">int</a> add_offset:<a href="../type/int.md">int</a> limit:<a href="../type/int.md">int</a> max_id:<a href="../type/int.md">int</a> min_id:<a href="../type/int.md">int</a> = <a href="../type/messages.Messages.md">messages.Messages</a>;
<a href="../method/messages.search.md">messages.search</a>#f288a275 flags:# peer:<a href="../type/InputPeer.md">InputPeer</a> q:<a href="../type/string.md">string</a> from_id:flags.0?<a href="../type/InputUser.md">InputUser</a> filter:<a href="../type/MessagesFilter.md">MessagesFilter</a> min_date:<a href="../type/int.md">int</a> max_date:<a href="../type/int.md">int</a> offset:<a href="../type/int.md">int</a> max_id:<a href="../type/int.md">int</a> limit:<a href="../type/int.md">int</a> = <a href="../type/messages.Messages.md">messages.Messages</a>;
<a href="../method/messages.searchGlobal.md">messages.searchGlobal</a>#9e3cacb0 q:<a href="../type/string.md">string</a> offset_date:<a href="../type/int.md">int</a> offset_peer:<a href="../type/InputPeer.md">InputPeer</a> offset_id:<a href="../type/int.md">int</a> limit:<a href="../type/int.md">int</a> = <a href="../type/messages.Messages.md">messages.Messages</a>;
<a href="../method/channels.getMessages.md">channels.getMessages</a>#93d7b347 channel:<a href="../type/InputChannel.md">InputChannel</a> id:Vector&lt;<a href="../type/int.md">int</a>&gt; = <a href="../type/messages.Messages.md">messages.Messages</a>;

</pre>

## Constructors

| Name | Description |
|------|-------------|
| [messages.messages](../constructor/messages.messages.md) | Sample Description |
| [messages.messagesSlice](../constructor/messages.messagesSlice.md) | Sample Description |
| [messages.channelMessages](../constructor/messages.channelMessages.md) | Sample Description |

## Methods

| Name | Description |
|------|-------------|
| [messages.getMessages](../method/messages.getMessages.md) | Sample Description |
| [messages.getHistory](../method/messages.getHistory.md) | Sample Description |
| [messages.search](../method/messages.search.md) | Sample Description |
| [messages.searchGlobal](../method/messages.searchGlobal.md) | Sample Description |
| [channels.getMessages](../method/channels.getMessages.md) | Sample Description |

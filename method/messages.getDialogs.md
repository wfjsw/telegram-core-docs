# messages.getDialogs

Returns the current user dialog list.

<pre>
<a href="../constructor/messages.dialogs.md">messages.dialogs</a>#15ba6c40 dialogs:Vector&lt;<a href="../type/Dialog.md">Dialog</a>&gt; messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/messages.Dialogs.md">messages.Dialogs</a>;
<a href="../constructor/messages.dialogsSlice.md">messages.dialogsSlice</a>#71e094f3 count:<a href="../type/int.md">int</a> dialogs:Vector&lt;<a href="../type/Dialog.md">Dialog</a>&gt; messages:Vector&lt;<a href="../type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/messages.Dialogs.md">messages.Dialogs</a>;

---functions---
<a href="../method/messages.getDialogs.md">messages.getDialogs</a>#191ba9c5 flags:# exclude_pinned:flags.0?<a href="../type/true.md">true</a> offset_date:<a href="../type/int.md">int</a> offset_id:<a href="../type/int.md">int</a> offset_peer:<a href="../type/InputPeer.md">InputPeer</a> limit:<a href="../type/int.md">int</a> = <a href="../type/messages.Dialogs.md">messages.Dialogs</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Param description |
| **exclude_pinned** | flags.0?<a href="../type/true.md">true</a> | Do not include pinned chat |
| **offset_date** | <a href="../type/int.md">int</a> | Param description |
| **offset_id** | <a href="../type/int.md">int</a> | Param description |
| **offset_peer** | <a href="../type/InputPeer.md">InputPeer</a> | Param description |
| **limit** | <a href="../type/int.md">int</a> | Number of list elements to be returned |

## Result

<a href="../type/messages.Dialogs.md">messages.Dialogs</a>


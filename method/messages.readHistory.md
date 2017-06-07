# messages.readHistory

Marks message history as read.

<pre>
<a href="../constructor/messages.affectedMessages.md">messages.affectedMessages</a>#84d19185 pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> = <a href="../type/messages.AffectedMessages.md">messages.AffectedMessages</a>;

---functions---
<a href="../method/messages.readHistory.md">messages.readHistory</a>#e306d3a peer:<a href="../type/InputPeer.md">InputPeer</a> max_id:<a href="../type/int.md">int</a> = <a href="../type/messages.AffectedMessages.md">messages.AffectedMessages</a>;</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **peer** | <a href="../type/InputPeer.md">InputPeer</a> | Target user or group |
| **max_id** | <a href="../type/int.md">int</a> | If a positive value is passed, only messages with identifiers less or equal than the given one will be read |

## Result

<a href="../type/messages.AffectedMessages.md">messages.AffectedMessages</a>


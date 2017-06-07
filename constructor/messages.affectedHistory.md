# messages.affectedHistory

Affected part of communication history with the user or in a chat.

<pre>
<a href="../constructor/messages.affectedHistory.md">messages.affectedHistory</a>#b45c69d1 pts:<a href="../type/int.md">int</a> pts_count:<a href="../type/int.md">int</a> offset:<a href="../type/int.md">int</a> = <a href="../type/messages.AffectedHistory.md">messages.AffectedHistory</a>;</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **pts** | <a href="../type/int.md">int</a> | Number of events occured in a text box |
| **pts_count** | <a href="../type/int.md">int</a> | Number of sent updates |
| **offset** | <a href="../type/int.md">int</a> | If a parameter contains positive value, it is necessary to repeat the method call using the given value; during the proceeding of all the history the value itself shall gradually decrease |

## Type

<a href="../type/messages.AffectedHistory.md">messages.AffectedHistory</a>

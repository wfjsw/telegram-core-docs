# channels.getAdminLog

Sample Description

<pre>
<a href="../constructor/channels.adminLogResults.md">channels.adminLogResults</a>#ed8af74d events:Vector&lt;<a href="../type/ChannelAdminLogEvent.md">ChannelAdminLogEvent</a>&gt; chats:Vector&lt;<a href="../type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="../type/User.md">User</a>&gt; = <a href="../type/channels.AdminLogResults.md">channels.AdminLogResults</a>;

---functions---
<a href="../method/channels.getAdminLog.md">channels.getAdminLog</a>#33ddf480 flags:# channel:<a href="../type/InputChannel.md">InputChannel</a> q:<a href="../type/string.md">string</a> events_filter:flags.0?<a href="../type/ChannelAdminLogEventsFilter.md">ChannelAdminLogEventsFilter</a> admins:flags.1?Vector&lt;<a href="../type/InputUser.md">InputUser</a>&gt; max_id:<a href="../type/long.md">long</a> min_id:<a href="../type/long.md">long</a> limit:<a href="../type/int.md">int</a> = <a href="../type/channels.AdminLogResults.md">channels.AdminLogResults</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Param description |
| **channel** | <a href="../type/InputChannel.md">InputChannel</a> | Param description |
| **q** | <a href="../type/string.md">string</a> | Param description |
| **events_filter** | flags.0?<a href="../type/ChannelAdminLogEventsFilter.md">ChannelAdminLogEventsFilter</a> | Param description |
| **admins** | flags.1?Vector&lt;<a href="../type/InputUser.md">InputUser</a>&gt; | Param description |
| **max_id** | <a href="../type/long.md">long</a> | Param description |
| **min_id** | <a href="../type/long.md">long</a> | Param description |
| **limit** | <a href="../type/int.md">int</a> | Param description |

## Result

<a href="../type/channels.AdminLogResults.md">channels.AdminLogResults</a>


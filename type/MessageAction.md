# MessageAction

Object describing actions connected to a service message.

<pre>
<a href="../constructor/messageActionEmpty.md">messageActionEmpty</a>#b6aef7b0 = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatCreate.md">messageActionChatCreate</a>#a6638b9a title:<a href="../type/string.md">string</a> users:Vector&lt;<a href="../type/int.md">int</a>&gt; = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatEditTitle.md">messageActionChatEditTitle</a>#b5a1ce5a title:<a href="../type/string.md">string</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatEditPhoto.md">messageActionChatEditPhoto</a>#7fcb13a8 photo:<a href="../type/Photo.md">Photo</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatDeletePhoto.md">messageActionChatDeletePhoto</a>#95e3fbef = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatAddUser.md">messageActionChatAddUser</a>#488a7337 users:Vector&lt;<a href="../type/int.md">int</a>&gt; = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatDeleteUser.md">messageActionChatDeleteUser</a>#b2ae9b0c user_id:<a href="../type/int.md">int</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatJoinedByLink.md">messageActionChatJoinedByLink</a>#f89cf5e8 inviter_id:<a href="../type/int.md">int</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChannelCreate.md">messageActionChannelCreate</a>#95d2ac92 title:<a href="../type/string.md">string</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChatMigrateTo.md">messageActionChatMigrateTo</a>#51bdb021 channel_id:<a href="../type/int.md">int</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionChannelMigrateFrom.md">messageActionChannelMigrateFrom</a>#b055eaee title:<a href="../type/string.md">string</a> chat_id:<a href="../type/int.md">int</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionPinMessage.md">messageActionPinMessage</a>#94bd38ed = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionHistoryClear.md">messageActionHistoryClear</a>#9fbab604 = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionGameScore.md">messageActionGameScore</a>#92a72876 game_id:<a href="../type/long.md">long</a> score:<a href="../type/int.md">int</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionPaymentSentMe.md">messageActionPaymentSentMe</a>#8f31b327 flags:<a href="../type/#.md">#</a> currency:<a href="../type/string.md">string</a> total_amount:<a href="../type/long.md">long</a> payload:<a href="../type/bytes.md">bytes</a> info:flags.0?<a href="../type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> shipping_option_id:flags.1?<a href="../type/string.md">string</a> charge:<a href="../type/PaymentCharge.md">PaymentCharge</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionPaymentSent.md">messageActionPaymentSent</a>#40699cd0 currency:<a href="../type/string.md">string</a> total_amount:<a href="../type/long.md">long</a> = <a href="../type/MessageAction.md">MessageAction</a>;
<a href="../constructor/messageActionPhoneCall.md">messageActionPhoneCall</a>#80e11a7f flags:<a href="../type/#.md">#</a> call_id:<a href="../type/long.md">long</a> reason:flags.0?<a href="../type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a> duration:flags.1?<a href="../type/int.md">int</a> = <a href="../type/MessageAction.md">MessageAction</a>;
</pre>

## Constructors

| Name | Description |
|------|-------------|
| [messageActionEmpty](../constructor/messageActionEmpty.md) | Empty constructor. |
| [messageActionChatCreate](../constructor/messageActionChatCreate.md) | Group created |
| [messageActionChatEditTitle](../constructor/messageActionChatEditTitle.md) | Sample Description |
| [messageActionChatEditPhoto](../constructor/messageActionChatEditPhoto.md) | Group profile changed |
| [messageActionChatDeletePhoto](../constructor/messageActionChatDeletePhoto.md) | Group profile photo removed. |
| [messageActionChatAddUser](../constructor/messageActionChatAddUser.md) | New member in the group |
| [messageActionChatDeleteUser](../constructor/messageActionChatDeleteUser.md) | User left the group. |
| [messageActionChatJoinedByLink](../constructor/messageActionChatJoinedByLink.md) | Sample Description |
| [messageActionChannelCreate](../constructor/messageActionChannelCreate.md) | Sample Description |
| [messageActionChatMigrateTo](../constructor/messageActionChatMigrateTo.md) | Sample Description |
| [messageActionChannelMigrateFrom](../constructor/messageActionChannelMigrateFrom.md) | Sample Description |
| [messageActionPinMessage](../constructor/messageActionPinMessage.md) | Sample Description |
| [messageActionHistoryClear](../constructor/messageActionHistoryClear.md) | Sample Description |
| [messageActionGameScore](../constructor/messageActionGameScore.md) | Sample Description |
| [messageActionPaymentSentMe](../constructor/messageActionPaymentSentMe.md) | Sample Description |
| [messageActionPaymentSent](../constructor/messageActionPaymentSent.md) | Sample Description |
| [messageActionPhoneCall](../constructor/messageActionPhoneCall.md) | Sample Description |


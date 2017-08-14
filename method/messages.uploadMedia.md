# messages.uploadMedia

Sample Description

<pre>
<a href="../constructor/messageMediaEmpty.md">messageMediaEmpty</a>#3ded6320 = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaPhoto.md">messageMediaPhoto</a>#b5223b0f flags:# photo:flags.0?<a href="../type/Photo.md">Photo</a> caption:flags.1?<a href="../type/string.md">string</a> ttl_seconds:flags.2?<a href="../type/int.md">int</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaGeo.md">messageMediaGeo</a>#56e0d474 geo:<a href="../type/GeoPoint.md">GeoPoint</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaContact.md">messageMediaContact</a>#5e7d2f39 phone_number:<a href="../type/string.md">string</a> first_name:<a href="../type/string.md">string</a> last_name:<a href="../type/string.md">string</a> user_id:<a href="../type/int.md">int</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaUnsupported.md">messageMediaUnsupported</a>#9f84f49e = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaDocument.md">messageMediaDocument</a>#7c4414d3 flags:# document:flags.0?<a href="../type/Document.md">Document</a> caption:flags.1?<a href="../type/string.md">string</a> ttl_seconds:flags.2?<a href="../type/int.md">int</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaWebPage.md">messageMediaWebPage</a>#a32dd600 webpage:<a href="../type/WebPage.md">WebPage</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaVenue.md">messageMediaVenue</a>#7912b71f geo:<a href="../type/GeoPoint.md">GeoPoint</a> title:<a href="../type/string.md">string</a> address:<a href="../type/string.md">string</a> provider:<a href="../type/string.md">string</a> venue_id:<a href="../type/string.md">string</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaGame.md">messageMediaGame</a>#fdb19008 game:<a href="../type/Game.md">Game</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
<a href="../constructor/messageMediaInvoice.md">messageMediaInvoice</a>#84551347 flags:# shipping_address_requested:flags.1?<a href="../type/true.md">true</a> test:flags.3?<a href="../type/true.md">true</a> title:<a href="../type/string.md">string</a> description:<a href="../type/string.md">string</a> photo:flags.0?<a href="../type/WebDocument.md">WebDocument</a> receipt_msg_id:flags.2?<a href="../type/int.md">int</a> currency:<a href="../type/string.md">string</a> total_amount:<a href="../type/long.md">long</a> start_param:<a href="../type/string.md">string</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;

---functions---
<a href="../method/messages.uploadMedia.md">messages.uploadMedia</a>#519bc2b1 peer:<a href="../type/InputPeer.md">InputPeer</a> media:<a href="../type/InputMedia.md">InputMedia</a> = <a href="../type/MessageMedia.md">MessageMedia</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **peer** | <a href="../type/InputPeer.md">InputPeer</a> | Param description |
| **media** | <a href="../type/InputMedia.md">InputMedia</a> | Param description |

## Result

<a href="../type/MessageMedia.md">MessageMedia</a>


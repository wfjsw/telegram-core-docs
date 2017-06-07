# Bool

Sample Description

<pre>
<a href="../constructor/boolFalse">boolFalse</a>#bc799737 = <a href="../type/Bool.md">Bool</a>;
<a href="../constructor/boolTrue">boolTrue</a>#997275b5 = <a href="../type/Bool.md">Bool</a>;

---functions---
<a href="../method/auth.logOut">auth.logOut</a>#5717da40 = <a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.resetAuthorizations">auth.resetAuthorizations</a>#9fab0d1a = <a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.sendInvites">auth.sendInvites</a>#771c1d97 phone_numbers:Vector&lt;<a href="../type/string.md">string</a>&gt; message:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.bindTempAuthKey">auth.bindTempAuthKey</a>#cdd42a05 perm_auth_key_id:<a href="../type/long.md">long</a> nonce:<a href="../type/long.md">long</a> expires_at:<a href="../type/int.md">int</a> encrypted_message:<a href="../type/bytes.md">bytes</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.cancelCode">auth.cancelCode</a>#1f040578 phone_number:<a href="../type/string.md">string</a> phone_code_hash:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.dropTempAuthKeys">auth.dropTempAuthKeys</a>#8e48a188 except_auth_keys:Vector&lt;<a href="../type/long.md">long</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.registerDevice">account.registerDevice</a>#637ea878 token_type:<a href="../type/int.md">int</a> token:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.unregisterDevice">account.unregisterDevice</a>#65c55b40 token_type:<a href="../type/int.md">int</a> token:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updateNotifySettings">account.updateNotifySettings</a>#84be5b93 peer:<a href="../type/InputNotifyPeer.md">InputNotifyPeer</a> settings:<a href="../type/InputPeerNotifySettings.md">InputPeerNotifySettings</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.resetNotifySettings">account.resetNotifySettings</a>#db7e1747 = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updateStatus">account.updateStatus</a>#6628562c offline:<a href="../type/Bool.md">Bool</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.reportPeer">account.reportPeer</a>#ae189d5f peer:<a href="../type/InputPeer.md">InputPeer</a> reason:<a href="../type/ReportReason.md">ReportReason</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.checkUsername">account.checkUsername</a>#2714d86c username:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.deleteAccount">account.deleteAccount</a>#418d4e0b reason:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.setAccountTTL">account.setAccountTTL</a>#2442485e ttl:<a href="../type/AccountDaysTTL.md">AccountDaysTTL</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updateDeviceLocked">account.updateDeviceLocked</a>#38df3532 period:<a href="../type/int.md">int</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.resetAuthorization">account.resetAuthorization</a>#df77f3bc hash:<a href="../type/long.md">long</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updatePasswordSettings">account.updatePasswordSettings</a>#fa7c4b86 current_password_hash:<a href="../type/bytes.md">bytes</a> new_settings:<a href="../type/account.PasswordInputSettings.md">account.PasswordInputSettings</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/account.confirmPhone">account.confirmPhone</a>#5f2178c3 phone_code_hash:<a href="../type/string.md">string</a> phone_code:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.deleteContacts">contacts.deleteContacts</a>#59ab389e id:Vector&lt;<a href="../type/InputUser.md">InputUser</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.block">contacts.block</a>#332b49fc id:<a href="../type/InputUser.md">InputUser</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.unblock">contacts.unblock</a>#e54100bd id:<a href="../type/InputUser.md">InputUser</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.resetTopPeerRating">contacts.resetTopPeerRating</a>#1ae373ac category:<a href="../type/TopPeerCategory.md">TopPeerCategory</a> peer:<a href="../type/InputPeer.md">InputPeer</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setTyping">messages.setTyping</a>#a3825e50 peer:<a href="../type/InputPeer.md">InputPeer</a> action:<a href="../type/SendMessageAction.md">SendMessageAction</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reportSpam">messages.reportSpam</a>#cf1592db peer:<a href="../type/InputPeer.md">InputPeer</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.hideReportSpam">messages.hideReportSpam</a>#a8f1709b peer:<a href="../type/InputPeer.md">InputPeer</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.discardEncryption">messages.discardEncryption</a>#edd923c5 chat_id:<a href="../type/int.md">int</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setEncryptedTyping">messages.setEncryptedTyping</a>#791451ed peer:<a href="../type/InputEncryptedChat.md">InputEncryptedChat</a> typing:<a href="../type/Bool.md">Bool</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.readEncryptedHistory">messages.readEncryptedHistory</a>#7f4b690a peer:<a href="../type/InputEncryptedChat.md">InputEncryptedChat</a> max_date:<a href="../type/int.md">int</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reportEncryptedSpam">messages.reportEncryptedSpam</a>#4b0c8c0f peer:<a href="../type/InputEncryptedChat.md">InputEncryptedChat</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.uninstallStickerSet">messages.uninstallStickerSet</a>#f96e55de stickerset:<a href="../type/InputStickerSet.md">InputStickerSet</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.editChatAdmin">messages.editChatAdmin</a>#a9e69f2e chat_id:<a href="../type/int.md">int</a> user_id:<a href="../type/InputUser.md">InputUser</a> is_admin:<a href="../type/Bool.md">Bool</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reorderStickerSets">messages.reorderStickerSets</a>#78337739 flags:<a href="../type/#.md">#</a> masks:<a href="../type/flags.0?true.md">flags.0?true</a> order:Vector&lt;<a href="../type/long.md">long</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.saveGif">messages.saveGif</a>#327a30cb id:<a href="../type/InputDocument.md">InputDocument</a> unsave:<a href="../type/Bool.md">Bool</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setInlineBotResults">messages.setInlineBotResults</a>#eb5ea206 flags:<a href="../type/#.md">#</a> gallery:<a href="../type/flags.0?true.md">flags.0?true</a> private:<a href="../type/flags.1?true.md">flags.1?true</a> query_id:<a href="../type/long.md">long</a> results:Vector&lt;<a href="../type/InputBotInlineResult.md">InputBotInlineResult</a>&gt; cache_time:<a href="../type/int.md">int</a> next_offset:<a href="../type/flags.2?string.md">flags.2?string</a> switch_pm:<a href="../type/flags.3?InlineBotSwitchPM.md">flags.3?InlineBotSwitchPM</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.editInlineBotMessage">messages.editInlineBotMessage</a>#130c2c85 flags:<a href="../type/#.md">#</a> no_webpage:<a href="../type/flags.1?true.md">flags.1?true</a> id:<a href="../type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> message:<a href="../type/flags.11?string.md">flags.11?string</a> reply_markup:<a href="../type/flags.2?ReplyMarkup.md">flags.2?ReplyMarkup</a> entities:Vector&lt;<a href="../type/flags.3?Vector.md">flags.3?Vector</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setBotCallbackAnswer">messages.setBotCallbackAnswer</a>#d58f130a flags:<a href="../type/#.md">#</a> alert:<a href="../type/flags.1?true.md">flags.1?true</a> query_id:<a href="../type/long.md">long</a> message:<a href="../type/flags.0?string.md">flags.0?string</a> url:<a href="../type/flags.2?string.md">flags.2?string</a> cache_time:<a href="../type/int.md">int</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.saveDraft">messages.saveDraft</a>#bc39e14b flags:<a href="../type/#.md">#</a> no_webpage:<a href="../type/flags.1?true.md">flags.1?true</a> reply_to_msg_id:<a href="../type/flags.0?int.md">flags.0?int</a> peer:<a href="../type/InputPeer.md">InputPeer</a> message:<a href="../type/string.md">string</a> entities:Vector&lt;<a href="../type/flags.3?Vector.md">flags.3?Vector</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.readFeaturedStickers">messages.readFeaturedStickers</a>#5b118126 id:Vector&lt;<a href="../type/long.md">long</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.saveRecentSticker">messages.saveRecentSticker</a>#392718f8 flags:<a href="../type/#.md">#</a> attached:<a href="../type/flags.0?true.md">flags.0?true</a> id:<a href="../type/InputDocument.md">InputDocument</a> unsave:<a href="../type/Bool.md">Bool</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.clearRecentStickers">messages.clearRecentStickers</a>#8999602d flags:<a href="../type/#.md">#</a> attached:<a href="../type/flags.0?true.md">flags.0?true</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setInlineGameScore">messages.setInlineGameScore</a>#15ad9f64 flags:<a href="../type/#.md">#</a> edit_message:<a href="../type/flags.0?true.md">flags.0?true</a> force:<a href="../type/flags.1?true.md">flags.1?true</a> id:<a href="../type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> user_id:<a href="../type/InputUser.md">InputUser</a> score:<a href="../type/int.md">int</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.toggleDialogPin">messages.toggleDialogPin</a>#3289be6a flags:<a href="../type/#.md">#</a> pinned:<a href="../type/flags.0?true.md">flags.0?true</a> peer:<a href="../type/InputPeer.md">InputPeer</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reorderPinnedDialogs">messages.reorderPinnedDialogs</a>#959ff644 flags:<a href="../type/#.md">#</a> force:<a href="../type/flags.0?true.md">flags.0?true</a> order:Vector&lt;<a href="../type/InputPeer.md">InputPeer</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setBotShippingResults">messages.setBotShippingResults</a>#e5f672fa flags:<a href="../type/#.md">#</a> query_id:<a href="../type/long.md">long</a> error:<a href="../type/flags.0?string.md">flags.0?string</a> shipping_options:Vector&lt;<a href="../type/flags.1?Vector.md">flags.1?Vector</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setBotPrecheckoutResults">messages.setBotPrecheckoutResults</a>#9c2dd95 flags:<a href="../type/#.md">#</a> success:<a href="../type/flags.1?true.md">flags.1?true</a> query_id:<a href="../type/long.md">long</a> error:<a href="../type/flags.0?string.md">flags.0?string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/upload.saveFilePart">upload.saveFilePart</a>#b304a621 file_id:<a href="../type/long.md">long</a> file_part:<a href="../type/int.md">int</a> bytes:<a href="../type/bytes.md">bytes</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/upload.saveBigFilePart">upload.saveBigFilePart</a>#de7b673d file_id:<a href="../type/long.md">long</a> file_part:<a href="../type/int.md">int</a> file_total_parts:<a href="../type/int.md">int</a> bytes:<a href="../type/bytes.md">bytes</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/upload.reuploadCdnFile">upload.reuploadCdnFile</a>#2e7a2020 file_token:<a href="../type/bytes.md">bytes</a> request_token:<a href="../type/bytes.md">bytes</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/help.saveAppLog">help.saveAppLog</a>#6f02f748 events:Vector&lt;<a href="../type/InputAppEvent.md">InputAppEvent</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/help.setBotUpdatesStatus">help.setBotUpdatesStatus</a>#ec22cfcd pending_updates_count:<a href="../type/int.md">int</a> message:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.readHistory">channels.readHistory</a>#cc104937 channel:<a href="../type/InputChannel.md">InputChannel</a> max_id:<a href="../type/int.md">int</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.reportSpam">channels.reportSpam</a>#fe087810 channel:<a href="../type/InputChannel.md">InputChannel</a> user_id:<a href="../type/InputUser.md">InputUser</a> id:Vector&lt;<a href="../type/int.md">int</a>&gt; = <a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.editAbout">channels.editAbout</a>#13e27f1e channel:<a href="../type/InputChannel.md">InputChannel</a> about:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.checkUsername">channels.checkUsername</a>#10e6bd2c channel:<a href="../type/InputChannel.md">InputChannel</a> username:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.updateUsername">channels.updateUsername</a>#3514b3de channel:<a href="../type/InputChannel.md">InputChannel</a> username:<a href="../type/string.md">string</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/bots.answerWebhookJSONQuery">bots.answerWebhookJSONQuery</a>#e6213f4d query_id:<a href="../type/long.md">long</a> data:<a href="../type/DataJSON.md">DataJSON</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/payments.clearSavedInfo">payments.clearSavedInfo</a>#d83d70c1 flags:<a href="../type/#.md">#</a> credentials:<a href="../type/flags.0?true.md">flags.0?true</a> info:<a href="../type/flags.1?true.md">flags.1?true</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/phone.receivedCall">phone.receivedCall</a>#17d54f61 peer:<a href="../type/InputPhoneCall.md">InputPhoneCall</a> = <a href="../type/Bool.md">Bool</a>;
<a href="../method/phone.saveCallDebug">phone.saveCallDebug</a>#277add7e peer:<a href="../type/InputPhoneCall.md">InputPhoneCall</a> debug:<a href="../type/DataJSON.md">DataJSON</a> = <a href="../type/Bool.md">Bool</a>;

</pre>

## Constructors

| Name | Description |
|------|-------------|
| [boolFalse](../constructor/boolFalse.md) | Sample Description |
| [boolTrue](../constructor/boolTrue.md) | Sample Description |

## Methods

| Name | Description |
|------|-------------|
| [auth.logOut](../method/auth.logOut.md) | Sample Description |
| [auth.resetAuthorizations](../method/auth.resetAuthorizations.md) | Sample Description |
| [auth.sendInvites](../method/auth.sendInvites.md) | Sample Description |
| [auth.bindTempAuthKey](../method/auth.bindTempAuthKey.md) | Sample Description |
| [auth.cancelCode](../method/auth.cancelCode.md) | Sample Description |
| [auth.dropTempAuthKeys](../method/auth.dropTempAuthKeys.md) | Sample Description |
| [account.registerDevice](../method/account.registerDevice.md) | Sample Description |
| [account.unregisterDevice](../method/account.unregisterDevice.md) | Sample Description |
| [account.updateNotifySettings](../method/account.updateNotifySettings.md) | Sample Description |
| [account.resetNotifySettings](../method/account.resetNotifySettings.md) | Sample Description |
| [account.updateStatus](../method/account.updateStatus.md) | Sample Description |
| [account.reportPeer](../method/account.reportPeer.md) | Sample Description |
| [account.checkUsername](../method/account.checkUsername.md) | Sample Description |
| [account.deleteAccount](../method/account.deleteAccount.md) | Sample Description |
| [account.setAccountTTL](../method/account.setAccountTTL.md) | Sample Description |
| [account.updateDeviceLocked](../method/account.updateDeviceLocked.md) | Sample Description |
| [account.resetAuthorization](../method/account.resetAuthorization.md) | Sample Description |
| [account.updatePasswordSettings](../method/account.updatePasswordSettings.md) | Sample Description |
| [account.confirmPhone](../method/account.confirmPhone.md) | Sample Description |
| [contacts.deleteContacts](../method/contacts.deleteContacts.md) | Sample Description |
| [contacts.block](../method/contacts.block.md) | Sample Description |
| [contacts.unblock](../method/contacts.unblock.md) | Sample Description |
| [contacts.resetTopPeerRating](../method/contacts.resetTopPeerRating.md) | Sample Description |
| [messages.setTyping](../method/messages.setTyping.md) | Sample Description |
| [messages.reportSpam](../method/messages.reportSpam.md) | Sample Description |
| [messages.hideReportSpam](../method/messages.hideReportSpam.md) | Sample Description |
| [messages.discardEncryption](../method/messages.discardEncryption.md) | Sample Description |
| [messages.setEncryptedTyping](../method/messages.setEncryptedTyping.md) | Sample Description |
| [messages.readEncryptedHistory](../method/messages.readEncryptedHistory.md) | Sample Description |
| [messages.reportEncryptedSpam](../method/messages.reportEncryptedSpam.md) | Sample Description |
| [messages.uninstallStickerSet](../method/messages.uninstallStickerSet.md) | Sample Description |
| [messages.editChatAdmin](../method/messages.editChatAdmin.md) | Sample Description |
| [messages.reorderStickerSets](../method/messages.reorderStickerSets.md) | Sample Description |
| [messages.saveGif](../method/messages.saveGif.md) | Sample Description |
| [messages.setInlineBotResults](../method/messages.setInlineBotResults.md) | Sample Description |
| [messages.editInlineBotMessage](../method/messages.editInlineBotMessage.md) | Sample Description |
| [messages.setBotCallbackAnswer](../method/messages.setBotCallbackAnswer.md) | Sample Description |
| [messages.saveDraft](../method/messages.saveDraft.md) | Sample Description |
| [messages.readFeaturedStickers](../method/messages.readFeaturedStickers.md) | Sample Description |
| [messages.saveRecentSticker](../method/messages.saveRecentSticker.md) | Sample Description |
| [messages.clearRecentStickers](../method/messages.clearRecentStickers.md) | Sample Description |
| [messages.setInlineGameScore](../method/messages.setInlineGameScore.md) | Sample Description |
| [messages.toggleDialogPin](../method/messages.toggleDialogPin.md) | Sample Description |
| [messages.reorderPinnedDialogs](../method/messages.reorderPinnedDialogs.md) | Sample Description |
| [messages.setBotShippingResults](../method/messages.setBotShippingResults.md) | Sample Description |
| [messages.setBotPrecheckoutResults](../method/messages.setBotPrecheckoutResults.md) | Sample Description |
| [upload.saveFilePart](../method/upload.saveFilePart.md) | Sample Description |
| [upload.saveBigFilePart](../method/upload.saveBigFilePart.md) | Sample Description |
| [upload.reuploadCdnFile](../method/upload.reuploadCdnFile.md) | Sample Description |
| [help.saveAppLog](../method/help.saveAppLog.md) | Sample Description |
| [help.setBotUpdatesStatus](../method/help.setBotUpdatesStatus.md) | Sample Description |
| [channels.readHistory](../method/channels.readHistory.md) | Sample Description |
| [channels.reportSpam](../method/channels.reportSpam.md) | Sample Description |
| [channels.editAbout](../method/channels.editAbout.md) | Sample Description |
| [channels.checkUsername](../method/channels.checkUsername.md) | Sample Description |
| [channels.updateUsername](../method/channels.updateUsername.md) | Sample Description |
| [bots.answerWebhookJSONQuery](../method/bots.answerWebhookJSONQuery.md) | Sample Description |
| [payments.clearSavedInfo](../method/payments.clearSavedInfo.md) | Sample Description |
| [phone.receivedCall](../method/phone.receivedCall.md) | Sample Description |
| [phone.saveCallDebug](../method/phone.saveCallDebug.md) | Sample Description |
# Bool

Sample Description

<pre>
<a href="../constructor/boolFalse">boolFalse</a>#bc799737 = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../constructor/boolTrue">boolTrue</a>#997275b5 = undefined<a href="../type/Bool.md">Bool</a>;

---functions---
<a href="../method/auth.logOut">auth.logOut</a>#5717da40 = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.resetAuthorizations">auth.resetAuthorizations</a>#9fab0d1a = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.sendInvites">auth.sendInvites</a>#771c1d97 phone_numbers:undefinedVector&lt;<a href="../type/string.md">string</a>&gt; message:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.bindTempAuthKey">auth.bindTempAuthKey</a>#cdd42a05 perm_auth_key_id:undefined<a href="../type/long.md">long</a> nonce:undefined<a href="../type/long.md">long</a> expires_at:undefined<a href="../type/int.md">int</a> encrypted_message:undefined<a href="../type/bytes.md">bytes</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.cancelCode">auth.cancelCode</a>#1f040578 phone_number:undefined<a href="../type/string.md">string</a> phone_code_hash:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/auth.dropTempAuthKeys">auth.dropTempAuthKeys</a>#8e48a188 except_auth_keys:undefinedVector&lt;<a href="../type/long.md">long</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.registerDevice">account.registerDevice</a>#637ea878 token_type:undefined<a href="../type/int.md">int</a> token:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.unregisterDevice">account.unregisterDevice</a>#65c55b40 token_type:undefined<a href="../type/int.md">int</a> token:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updateNotifySettings">account.updateNotifySettings</a>#84be5b93 peer:undefined<a href="../type/InputNotifyPeer.md">InputNotifyPeer</a> settings:undefined<a href="../type/InputPeerNotifySettings.md">InputPeerNotifySettings</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.resetNotifySettings">account.resetNotifySettings</a>#db7e1747 = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updateStatus">account.updateStatus</a>#6628562c offline:undefined<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.reportPeer">account.reportPeer</a>#ae189d5f peer:undefined<a href="../type/InputPeer.md">InputPeer</a> reason:undefined<a href="../type/ReportReason.md">ReportReason</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.checkUsername">account.checkUsername</a>#2714d86c username:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.deleteAccount">account.deleteAccount</a>#418d4e0b reason:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.setAccountTTL">account.setAccountTTL</a>#2442485e ttl:undefined<a href="../type/AccountDaysTTL.md">AccountDaysTTL</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updateDeviceLocked">account.updateDeviceLocked</a>#38df3532 period:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.resetAuthorization">account.resetAuthorization</a>#df77f3bc hash:undefined<a href="../type/long.md">long</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.updatePasswordSettings">account.updatePasswordSettings</a>#fa7c4b86 current_password_hash:undefined<a href="../type/bytes.md">bytes</a> new_settings:undefined<a href="../type/account.PasswordInputSettings.md">account.PasswordInputSettings</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/account.confirmPhone">account.confirmPhone</a>#5f2178c3 phone_code_hash:undefined<a href="../type/string.md">string</a> phone_code:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.deleteContacts">contacts.deleteContacts</a>#59ab389e id:undefinedVector&lt;<a href="../type/InputUser.md">InputUser</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.block">contacts.block</a>#332b49fc id:undefined<a href="../type/InputUser.md">InputUser</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.unblock">contacts.unblock</a>#e54100bd id:undefined<a href="../type/InputUser.md">InputUser</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/contacts.resetTopPeerRating">contacts.resetTopPeerRating</a>#1ae373ac category:undefined<a href="../type/TopPeerCategory.md">TopPeerCategory</a> peer:undefined<a href="../type/InputPeer.md">InputPeer</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setTyping">messages.setTyping</a>#a3825e50 peer:undefined<a href="../type/InputPeer.md">InputPeer</a> action:undefined<a href="../type/SendMessageAction.md">SendMessageAction</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reportSpam">messages.reportSpam</a>#cf1592db peer:undefined<a href="../type/InputPeer.md">InputPeer</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.hideReportSpam">messages.hideReportSpam</a>#a8f1709b peer:undefined<a href="../type/InputPeer.md">InputPeer</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.discardEncryption">messages.discardEncryption</a>#edd923c5 chat_id:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setEncryptedTyping">messages.setEncryptedTyping</a>#791451ed peer:undefined<a href="../type/InputEncryptedChat.md">InputEncryptedChat</a> typing:undefined<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.readEncryptedHistory">messages.readEncryptedHistory</a>#7f4b690a peer:undefined<a href="../type/InputEncryptedChat.md">InputEncryptedChat</a> max_date:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reportEncryptedSpam">messages.reportEncryptedSpam</a>#4b0c8c0f peer:undefined<a href="../type/InputEncryptedChat.md">InputEncryptedChat</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.uninstallStickerSet">messages.uninstallStickerSet</a>#f96e55de stickerset:undefined<a href="../type/InputStickerSet.md">InputStickerSet</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.editChatAdmin">messages.editChatAdmin</a>#a9e69f2e chat_id:undefined<a href="../type/int.md">int</a> user_id:undefined<a href="../type/InputUser.md">InputUser</a> is_admin:undefined<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reorderStickerSets">messages.reorderStickerSets</a>#78337739 flags:undefined<a href="../type/#.md">#</a> masks:flags.0?<a href="../type/true.md">true</a> order:undefinedVector&lt;<a href="../type/long.md">long</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.saveGif">messages.saveGif</a>#327a30cb id:undefined<a href="../type/InputDocument.md">InputDocument</a> unsave:undefined<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setInlineBotResults">messages.setInlineBotResults</a>#eb5ea206 flags:undefined<a href="../type/#.md">#</a> gallery:flags.0?<a href="../type/true.md">true</a> private:flags.1?<a href="../type/true.md">true</a> query_id:undefined<a href="../type/long.md">long</a> results:undefinedVector&lt;<a href="../type/InputBotInlineResult.md">InputBotInlineResult</a>&gt; cache_time:undefined<a href="../type/int.md">int</a> next_offset:flags.2?<a href="../type/string.md">string</a> switch_pm:flags.3?<a href="../type/InlineBotSwitchPM.md">InlineBotSwitchPM</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.editInlineBotMessage">messages.editInlineBotMessage</a>#130c2c85 flags:undefined<a href="../type/#.md">#</a> no_webpage:flags.1?<a href="../type/true.md">true</a> id:undefined<a href="../type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> message:flags.11?<a href="../type/string.md">string</a> reply_markup:flags.2?<a href="../type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.3?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setBotCallbackAnswer">messages.setBotCallbackAnswer</a>#d58f130a flags:undefined<a href="../type/#.md">#</a> alert:flags.1?<a href="../type/true.md">true</a> query_id:undefined<a href="../type/long.md">long</a> message:flags.0?<a href="../type/string.md">string</a> url:flags.2?<a href="../type/string.md">string</a> cache_time:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.saveDraft">messages.saveDraft</a>#bc39e14b flags:undefined<a href="../type/#.md">#</a> no_webpage:flags.1?<a href="../type/true.md">true</a> reply_to_msg_id:flags.0?<a href="../type/int.md">int</a> peer:undefined<a href="../type/InputPeer.md">InputPeer</a> message:undefined<a href="../type/string.md">string</a> entities:flags.3?Vector&lt;<a href="../type/MessageEntity.md">MessageEntity</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.readFeaturedStickers">messages.readFeaturedStickers</a>#5b118126 id:undefinedVector&lt;<a href="../type/long.md">long</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.saveRecentSticker">messages.saveRecentSticker</a>#392718f8 flags:undefined<a href="../type/#.md">#</a> attached:flags.0?<a href="../type/true.md">true</a> id:undefined<a href="../type/InputDocument.md">InputDocument</a> unsave:undefined<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.clearRecentStickers">messages.clearRecentStickers</a>#8999602d flags:undefined<a href="../type/#.md">#</a> attached:flags.0?<a href="../type/true.md">true</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setInlineGameScore">messages.setInlineGameScore</a>#15ad9f64 flags:undefined<a href="../type/#.md">#</a> edit_message:flags.0?<a href="../type/true.md">true</a> force:flags.1?<a href="../type/true.md">true</a> id:undefined<a href="../type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> user_id:undefined<a href="../type/InputUser.md">InputUser</a> score:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.toggleDialogPin">messages.toggleDialogPin</a>#3289be6a flags:undefined<a href="../type/#.md">#</a> pinned:flags.0?<a href="../type/true.md">true</a> peer:undefined<a href="../type/InputPeer.md">InputPeer</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.reorderPinnedDialogs">messages.reorderPinnedDialogs</a>#959ff644 flags:undefined<a href="../type/#.md">#</a> force:flags.0?<a href="../type/true.md">true</a> order:undefinedVector&lt;<a href="../type/InputPeer.md">InputPeer</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setBotShippingResults">messages.setBotShippingResults</a>#e5f672fa flags:undefined<a href="../type/#.md">#</a> query_id:undefined<a href="../type/long.md">long</a> error:flags.0?<a href="../type/string.md">string</a> shipping_options:flags.1?Vector&lt;<a href="../type/ShippingOption.md">ShippingOption</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/messages.setBotPrecheckoutResults">messages.setBotPrecheckoutResults</a>#9c2dd95 flags:undefined<a href="../type/#.md">#</a> success:flags.1?<a href="../type/true.md">true</a> query_id:undefined<a href="../type/long.md">long</a> error:flags.0?<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/upload.saveFilePart">upload.saveFilePart</a>#b304a621 file_id:undefined<a href="../type/long.md">long</a> file_part:undefined<a href="../type/int.md">int</a> bytes:undefined<a href="../type/bytes.md">bytes</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/upload.saveBigFilePart">upload.saveBigFilePart</a>#de7b673d file_id:undefined<a href="../type/long.md">long</a> file_part:undefined<a href="../type/int.md">int</a> file_total_parts:undefined<a href="../type/int.md">int</a> bytes:undefined<a href="../type/bytes.md">bytes</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/upload.reuploadCdnFile">upload.reuploadCdnFile</a>#2e7a2020 file_token:undefined<a href="../type/bytes.md">bytes</a> request_token:undefined<a href="../type/bytes.md">bytes</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/help.saveAppLog">help.saveAppLog</a>#6f02f748 events:undefinedVector&lt;<a href="../type/InputAppEvent.md">InputAppEvent</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/help.setBotUpdatesStatus">help.setBotUpdatesStatus</a>#ec22cfcd pending_updates_count:undefined<a href="../type/int.md">int</a> message:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.readHistory">channels.readHistory</a>#cc104937 channel:undefined<a href="../type/InputChannel.md">InputChannel</a> max_id:undefined<a href="../type/int.md">int</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.reportSpam">channels.reportSpam</a>#fe087810 channel:undefined<a href="../type/InputChannel.md">InputChannel</a> user_id:undefined<a href="../type/InputUser.md">InputUser</a> id:undefinedVector&lt;<a href="../type/int.md">int</a>&gt; = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.editAbout">channels.editAbout</a>#13e27f1e channel:undefined<a href="../type/InputChannel.md">InputChannel</a> about:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.checkUsername">channels.checkUsername</a>#10e6bd2c channel:undefined<a href="../type/InputChannel.md">InputChannel</a> username:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/channels.updateUsername">channels.updateUsername</a>#3514b3de channel:undefined<a href="../type/InputChannel.md">InputChannel</a> username:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/bots.answerWebhookJSONQuery">bots.answerWebhookJSONQuery</a>#e6213f4d query_id:undefined<a href="../type/long.md">long</a> data:undefined<a href="../type/DataJSON.md">DataJSON</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/payments.clearSavedInfo">payments.clearSavedInfo</a>#d83d70c1 flags:undefined<a href="../type/#.md">#</a> credentials:flags.0?<a href="../type/true.md">true</a> info:flags.1?<a href="../type/true.md">true</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/phone.receivedCall">phone.receivedCall</a>#17d54f61 peer:undefined<a href="../type/InputPhoneCall.md">InputPhoneCall</a> = undefined<a href="../type/Bool.md">Bool</a>;
<a href="../method/phone.saveCallDebug">phone.saveCallDebug</a>#277add7e peer:undefined<a href="../type/InputPhoneCall.md">InputPhoneCall</a> debug:undefined<a href="../type/DataJSON.md">DataJSON</a> = undefined<a href="../type/Bool.md">Bool</a>;

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

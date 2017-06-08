# Current TL-schema

Below you will find [the current TL-schema](schema.tl). 

See also the [detailed schema in JSON »](schema.json)

<pre>
///////////////////////////////
///////// Main application API
///////////////////////////////

---types---

<a href="./constructor/boolFalse.md">boolFalse</a>#bc799737 = <a href="./type/Bool.md">Bool</a>;
<a href="./constructor/boolTrue.md">boolTrue</a>#997275b5 = <a href="./type/Bool.md">Bool</a>;

<a href="./constructor/true.md">true</a>#3fedd339 = <a href="./type/True.md">True</a>;

<a href="./constructor/vector.md">vector</a>#1cb5c415 = <a href="./type/t.md">t</a>;

<a href="./constructor/error.md">error</a>#c4b9f9bb code:<a href="./type/int.md">int</a> text:<a href="./type/string.md">string</a> = <a href="./type/Error.md">Error</a>;

<a href="./constructor/null.md">null</a>#56730bcc = <a href="./type/Null.md">Null</a>;

<a href="./constructor/inputPeerEmpty.md">inputPeerEmpty</a>#7f3b18ea = <a href="./type/InputPeer.md">InputPeer</a>;
<a href="./constructor/inputPeerSelf.md">inputPeerSelf</a>#7da07ec9 = <a href="./type/InputPeer.md">InputPeer</a>;
<a href="./constructor/inputPeerChat.md">inputPeerChat</a>#179be863 chat_id:<a href="./type/int.md">int</a> = <a href="./type/InputPeer.md">InputPeer</a>;
<a href="./constructor/inputPeerUser.md">inputPeerUser</a>#7b8e7de6 user_id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputPeer.md">InputPeer</a>;
<a href="./constructor/inputPeerChannel.md">inputPeerChannel</a>#20adaef8 channel_id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputPeer.md">InputPeer</a>;

<a href="./constructor/inputUserEmpty.md">inputUserEmpty</a>#b98886cf = <a href="./type/InputUser.md">InputUser</a>;
<a href="./constructor/inputUserSelf.md">inputUserSelf</a>#f7c1b13f = <a href="./type/InputUser.md">InputUser</a>;
<a href="./constructor/inputUser.md">inputUser</a>#d8292816 user_id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputUser.md">InputUser</a>;

<a href="./constructor/inputPhoneContact.md">inputPhoneContact</a>#f392b7f4 client_id:<a href="./type/long.md">long</a> phone:<a href="./type/string.md">string</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> = <a href="./type/InputContact.md">InputContact</a>;

<a href="./constructor/inputFile.md">inputFile</a>#f52ff27f id:<a href="./type/long.md">long</a> parts:<a href="./type/int.md">int</a> name:<a href="./type/string.md">string</a> md5_checksum:<a href="./type/string.md">string</a> = <a href="./type/InputFile.md">InputFile</a>;
<a href="./constructor/inputFileBig.md">inputFileBig</a>#fa4f0bb5 id:<a href="./type/long.md">long</a> parts:<a href="./type/int.md">int</a> name:<a href="./type/string.md">string</a> = <a href="./type/InputFile.md">InputFile</a>;

<a href="./constructor/inputMediaEmpty.md">inputMediaEmpty</a>#9664f57f = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaUploadedPhoto.md">inputMediaUploadedPhoto</a>#630c9af1 flags:# file:<a href="./type/InputFile.md">InputFile</a> caption:<a href="./type/string.md">string</a> stickers:flags.0?Vector&lt;<a href="./type/InputDocument.md">InputDocument</a>&gt; = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaPhoto.md">inputMediaPhoto</a>#e9bfb4f3 id:<a href="./type/InputPhoto.md">InputPhoto</a> caption:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaGeoPoint.md">inputMediaGeoPoint</a>#f9c44144 geo_point:<a href="./type/InputGeoPoint.md">InputGeoPoint</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaContact.md">inputMediaContact</a>#a6e45987 phone_number:<a href="./type/string.md">string</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaUploadedDocument.md">inputMediaUploadedDocument</a>#d070f1e9 flags:# file:<a href="./type/InputFile.md">InputFile</a> mime_type:<a href="./type/string.md">string</a> attributes:Vector&lt;<a href="./type/DocumentAttribute.md">DocumentAttribute</a>&gt; caption:<a href="./type/string.md">string</a> stickers:flags.0?Vector&lt;<a href="./type/InputDocument.md">InputDocument</a>&gt; = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaUploadedThumbDocument.md">inputMediaUploadedThumbDocument</a>#50d88cae flags:# file:<a href="./type/InputFile.md">InputFile</a> thumb:<a href="./type/InputFile.md">InputFile</a> mime_type:<a href="./type/string.md">string</a> attributes:Vector&lt;<a href="./type/DocumentAttribute.md">DocumentAttribute</a>&gt; caption:<a href="./type/string.md">string</a> stickers:flags.0?Vector&lt;<a href="./type/InputDocument.md">InputDocument</a>&gt; = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaDocument.md">inputMediaDocument</a>#1a77f29c id:<a href="./type/InputDocument.md">InputDocument</a> caption:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaVenue.md">inputMediaVenue</a>#2827a81a geo_point:<a href="./type/InputGeoPoint.md">InputGeoPoint</a> title:<a href="./type/string.md">string</a> address:<a href="./type/string.md">string</a> provider:<a href="./type/string.md">string</a> venue_id:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaGifExternal.md">inputMediaGifExternal</a>#4843b0fd url:<a href="./type/string.md">string</a> q:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaPhotoExternal.md">inputMediaPhotoExternal</a>#b55f4f18 url:<a href="./type/string.md">string</a> caption:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaDocumentExternal.md">inputMediaDocumentExternal</a>#e5e9607c url:<a href="./type/string.md">string</a> caption:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaGame.md">inputMediaGame</a>#d33f43f3 id:<a href="./type/InputGame.md">InputGame</a> = <a href="./type/InputMedia.md">InputMedia</a>;
<a href="./constructor/inputMediaInvoice.md">inputMediaInvoice</a>#92153685 flags:# title:<a href="./type/string.md">string</a> description:<a href="./type/string.md">string</a> photo:flags.0?<a href="./type/InputWebDocument.md">InputWebDocument</a> invoice:<a href="./type/Invoice.md">Invoice</a> payload:<a href="./type/bytes.md">bytes</a> provider:<a href="./type/string.md">string</a> start_param:<a href="./type/string.md">string</a> = <a href="./type/InputMedia.md">InputMedia</a>;

<a href="./constructor/inputChatPhotoEmpty.md">inputChatPhotoEmpty</a>#1ca48f57 = <a href="./type/InputChatPhoto.md">InputChatPhoto</a>;
<a href="./constructor/inputChatUploadedPhoto.md">inputChatUploadedPhoto</a>#927c55b4 file:<a href="./type/InputFile.md">InputFile</a> = <a href="./type/InputChatPhoto.md">InputChatPhoto</a>;
<a href="./constructor/inputChatPhoto.md">inputChatPhoto</a>#8953ad37 id:<a href="./type/InputPhoto.md">InputPhoto</a> = <a href="./type/InputChatPhoto.md">InputChatPhoto</a>;

<a href="./constructor/inputGeoPointEmpty.md">inputGeoPointEmpty</a>#e4c123d6 = <a href="./type/InputGeoPoint.md">InputGeoPoint</a>;
<a href="./constructor/inputGeoPoint.md">inputGeoPoint</a>#f3b7acc9 lat:<a href="./type/double.md">double</a> long:<a href="./type/double.md">double</a> = <a href="./type/InputGeoPoint.md">InputGeoPoint</a>;

<a href="./constructor/inputPhotoEmpty.md">inputPhotoEmpty</a>#1cd7bf0d = <a href="./type/InputPhoto.md">InputPhoto</a>;
<a href="./constructor/inputPhoto.md">inputPhoto</a>#fb95c6c4 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputPhoto.md">InputPhoto</a>;

<a href="./constructor/inputFileLocation.md">inputFileLocation</a>#14637196 volume_id:<a href="./type/long.md">long</a> local_id:<a href="./type/int.md">int</a> secret:<a href="./type/long.md">long</a> = <a href="./type/InputFileLocation.md">InputFileLocation</a>;
<a href="./constructor/inputEncryptedFileLocation.md">inputEncryptedFileLocation</a>#f5235d55 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputFileLocation.md">InputFileLocation</a>;
<a href="./constructor/inputDocumentFileLocation.md">inputDocumentFileLocation</a>#430f0724 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> version:<a href="./type/int.md">int</a> = <a href="./type/InputFileLocation.md">InputFileLocation</a>;

<a href="./constructor/inputAppEvent.md">inputAppEvent</a>#770656a8 time:<a href="./type/double.md">double</a> type:<a href="./type/string.md">string</a> peer:<a href="./type/long.md">long</a> data:<a href="./type/string.md">string</a> = <a href="./type/InputAppEvent.md">InputAppEvent</a>;

<a href="./constructor/peerUser.md">peerUser</a>#9db1bc6d user_id:<a href="./type/int.md">int</a> = <a href="./type/Peer.md">Peer</a>;
<a href="./constructor/peerChat.md">peerChat</a>#bad0e5bb chat_id:<a href="./type/int.md">int</a> = <a href="./type/Peer.md">Peer</a>;
<a href="./constructor/peerChannel.md">peerChannel</a>#bddde532 channel_id:<a href="./type/int.md">int</a> = <a href="./type/Peer.md">Peer</a>;

<a href="./constructor/storage.fileUnknown.md">storage.fileUnknown</a>#aa963b05 = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.filePartial.md">storage.filePartial</a>#40bc6f52 = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.fileJpeg.md">storage.fileJpeg</a>#7efe0e = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.fileGif.md">storage.fileGif</a>#cae1aadf = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.filePng.md">storage.filePng</a>#a4f63c0 = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.filePdf.md">storage.filePdf</a>#ae1e508d = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.fileMp3.md">storage.fileMp3</a>#528a0677 = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.fileMov.md">storage.fileMov</a>#4b09ebbc = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.fileMp4.md">storage.fileMp4</a>#b3cea0e4 = <a href="./type/storage.FileType.md">storage.FileType</a>;
<a href="./constructor/storage.fileWebp.md">storage.fileWebp</a>#1081464c = <a href="./type/storage.FileType.md">storage.FileType</a>;

<a href="./constructor/fileLocationUnavailable.md">fileLocationUnavailable</a>#7c596b46 volume_id:<a href="./type/long.md">long</a> local_id:<a href="./type/int.md">int</a> secret:<a href="./type/long.md">long</a> = <a href="./type/FileLocation.md">FileLocation</a>;
<a href="./constructor/fileLocation.md">fileLocation</a>#53d69076 dc_id:<a href="./type/int.md">int</a> volume_id:<a href="./type/long.md">long</a> local_id:<a href="./type/int.md">int</a> secret:<a href="./type/long.md">long</a> = <a href="./type/FileLocation.md">FileLocation</a>;

<a href="./constructor/userEmpty.md">userEmpty</a>#200250ba id:<a href="./type/int.md">int</a> = <a href="./type/User.md">User</a>;
<a href="./constructor/user.md">user</a>#2e13f4c3 flags:# self:flags.10?<a href="./type/true.md">true</a> contact:flags.11?<a href="./type/true.md">true</a> mutual_contact:flags.12?<a href="./type/true.md">true</a> deleted:flags.13?<a href="./type/true.md">true</a> bot:flags.14?<a href="./type/true.md">true</a> bot_chat_history:flags.15?<a href="./type/true.md">true</a> bot_nochats:flags.16?<a href="./type/true.md">true</a> verified:flags.17?<a href="./type/true.md">true</a> restricted:flags.18?<a href="./type/true.md">true</a> min:flags.20?<a href="./type/true.md">true</a> bot_inline_geo:flags.21?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> access_hash:flags.0?<a href="./type/long.md">long</a> first_name:flags.1?<a href="./type/string.md">string</a> last_name:flags.2?<a href="./type/string.md">string</a> username:flags.3?<a href="./type/string.md">string</a> phone:flags.4?<a href="./type/string.md">string</a> photo:flags.5?<a href="./type/UserProfilePhoto.md">UserProfilePhoto</a> status:flags.6?<a href="./type/UserStatus.md">UserStatus</a> bot_info_version:flags.14?<a href="./type/int.md">int</a> restriction_reason:flags.18?<a href="./type/string.md">string</a> bot_inline_placeholder:flags.19?<a href="./type/string.md">string</a> lang_code:flags.22?<a href="./type/string.md">string</a> = <a href="./type/User.md">User</a>;

<a href="./constructor/userProfilePhotoEmpty.md">userProfilePhotoEmpty</a>#4f11bae1 = <a href="./type/UserProfilePhoto.md">UserProfilePhoto</a>;
<a href="./constructor/userProfilePhoto.md">userProfilePhoto</a>#d559d8c8 photo_id:<a href="./type/long.md">long</a> photo_small:<a href="./type/FileLocation.md">FileLocation</a> photo_big:<a href="./type/FileLocation.md">FileLocation</a> = <a href="./type/UserProfilePhoto.md">UserProfilePhoto</a>;

<a href="./constructor/userStatusEmpty.md">userStatusEmpty</a>#9d05049 = <a href="./type/UserStatus.md">UserStatus</a>;
<a href="./constructor/userStatusOnline.md">userStatusOnline</a>#edb93949 expires:<a href="./type/int.md">int</a> = <a href="./type/UserStatus.md">UserStatus</a>;
<a href="./constructor/userStatusOffline.md">userStatusOffline</a>#8c703f was_online:<a href="./type/int.md">int</a> = <a href="./type/UserStatus.md">UserStatus</a>;
<a href="./constructor/userStatusRecently.md">userStatusRecently</a>#e26f42f1 = <a href="./type/UserStatus.md">UserStatus</a>;
<a href="./constructor/userStatusLastWeek.md">userStatusLastWeek</a>#7bf09fc = <a href="./type/UserStatus.md">UserStatus</a>;
<a href="./constructor/userStatusLastMonth.md">userStatusLastMonth</a>#77ebc742 = <a href="./type/UserStatus.md">UserStatus</a>;

<a href="./constructor/chatEmpty.md">chatEmpty</a>#9ba2d800 id:<a href="./type/int.md">int</a> = <a href="./type/Chat.md">Chat</a>;
<a href="./constructor/chat.md">chat</a>#d91cdd54 flags:# creator:flags.0?<a href="./type/true.md">true</a> kicked:flags.1?<a href="./type/true.md">true</a> left:flags.2?<a href="./type/true.md">true</a> admins_enabled:flags.3?<a href="./type/true.md">true</a> admin:flags.4?<a href="./type/true.md">true</a> deactivated:flags.5?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> title:<a href="./type/string.md">string</a> photo:<a href="./type/ChatPhoto.md">ChatPhoto</a> participants_count:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> version:<a href="./type/int.md">int</a> migrated_to:flags.6?<a href="./type/InputChannel.md">InputChannel</a> = <a href="./type/Chat.md">Chat</a>;
<a href="./constructor/chatForbidden.md">chatForbidden</a>#7328bdb id:<a href="./type/int.md">int</a> title:<a href="./type/string.md">string</a> = <a href="./type/Chat.md">Chat</a>;
<a href="./constructor/channel.md">channel</a>#a14dca52 flags:# creator:flags.0?<a href="./type/true.md">true</a> kicked:flags.1?<a href="./type/true.md">true</a> left:flags.2?<a href="./type/true.md">true</a> editor:flags.3?<a href="./type/true.md">true</a> moderator:flags.4?<a href="./type/true.md">true</a> broadcast:flags.5?<a href="./type/true.md">true</a> verified:flags.7?<a href="./type/true.md">true</a> megagroup:flags.8?<a href="./type/true.md">true</a> restricted:flags.9?<a href="./type/true.md">true</a> democracy:flags.10?<a href="./type/true.md">true</a> signatures:flags.11?<a href="./type/true.md">true</a> min:flags.12?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> access_hash:flags.13?<a href="./type/long.md">long</a> title:<a href="./type/string.md">string</a> username:flags.6?<a href="./type/string.md">string</a> photo:<a href="./type/ChatPhoto.md">ChatPhoto</a> date:<a href="./type/int.md">int</a> version:<a href="./type/int.md">int</a> restriction_reason:flags.9?<a href="./type/string.md">string</a> = <a href="./type/Chat.md">Chat</a>;
<a href="./constructor/channelForbidden.md">channelForbidden</a>#8537784f flags:# broadcast:flags.5?<a href="./type/true.md">true</a> megagroup:flags.8?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> title:<a href="./type/string.md">string</a> = <a href="./type/Chat.md">Chat</a>;

<a href="./constructor/chatFull.md">chatFull</a>#2e02a614 id:<a href="./type/int.md">int</a> participants:<a href="./type/ChatParticipants.md">ChatParticipants</a> chat_photo:<a href="./type/Photo.md">Photo</a> notify_settings:<a href="./type/PeerNotifySettings.md">PeerNotifySettings</a> exported_invite:<a href="./type/ExportedChatInvite.md">ExportedChatInvite</a> bot_info:Vector&lt;<a href="./type/BotInfo.md">BotInfo</a>&gt; = <a href="./type/ChatFull.md">ChatFull</a>;
<a href="./constructor/channelFull.md">channelFull</a>#c3d5512f flags:# can_view_participants:flags.3?<a href="./type/true.md">true</a> can_set_username:flags.6?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> about:<a href="./type/string.md">string</a> participants_count:flags.0?<a href="./type/int.md">int</a> admins_count:flags.1?<a href="./type/int.md">int</a> kicked_count:flags.2?<a href="./type/int.md">int</a> read_inbox_max_id:<a href="./type/int.md">int</a> read_outbox_max_id:<a href="./type/int.md">int</a> unread_count:<a href="./type/int.md">int</a> chat_photo:<a href="./type/Photo.md">Photo</a> notify_settings:<a href="./type/PeerNotifySettings.md">PeerNotifySettings</a> exported_invite:<a href="./type/ExportedChatInvite.md">ExportedChatInvite</a> bot_info:Vector&lt;<a href="./type/BotInfo.md">BotInfo</a>&gt; migrated_from_chat_id:flags.4?<a href="./type/int.md">int</a> migrated_from_max_id:flags.4?<a href="./type/int.md">int</a> pinned_msg_id:flags.5?<a href="./type/int.md">int</a> = <a href="./type/ChatFull.md">ChatFull</a>;

<a href="./constructor/chatParticipant.md">chatParticipant</a>#c8d7493e user_id:<a href="./type/int.md">int</a> inviter_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChatParticipant.md">ChatParticipant</a>;
<a href="./constructor/chatParticipantCreator.md">chatParticipantCreator</a>#da13538a user_id:<a href="./type/int.md">int</a> = <a href="./type/ChatParticipant.md">ChatParticipant</a>;
<a href="./constructor/chatParticipantAdmin.md">chatParticipantAdmin</a>#e2d6e436 user_id:<a href="./type/int.md">int</a> inviter_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChatParticipant.md">ChatParticipant</a>;

<a href="./constructor/chatParticipantsForbidden.md">chatParticipantsForbidden</a>#fc900c2b flags:# chat_id:<a href="./type/int.md">int</a> self_participant:flags.0?<a href="./type/ChatParticipant.md">ChatParticipant</a> = <a href="./type/ChatParticipants.md">ChatParticipants</a>;
<a href="./constructor/chatParticipants.md">chatParticipants</a>#3f460fed chat_id:<a href="./type/int.md">int</a> participants:Vector&lt;<a href="./type/ChatParticipant.md">ChatParticipant</a>&gt; version:<a href="./type/int.md">int</a> = <a href="./type/ChatParticipants.md">ChatParticipants</a>;

<a href="./constructor/chatPhotoEmpty.md">chatPhotoEmpty</a>#37c1011c = <a href="./type/ChatPhoto.md">ChatPhoto</a>;
<a href="./constructor/chatPhoto.md">chatPhoto</a>#6153276a photo_small:<a href="./type/FileLocation.md">FileLocation</a> photo_big:<a href="./type/FileLocation.md">FileLocation</a> = <a href="./type/ChatPhoto.md">ChatPhoto</a>;

<a href="./constructor/messageEmpty.md">messageEmpty</a>#83e5de54 id:<a href="./type/int.md">int</a> = <a href="./type/Message.md">Message</a>;
<a href="./constructor/message.md">message</a>#c09be45f flags:# out:flags.1?<a href="./type/true.md">true</a> mentioned:flags.4?<a href="./type/true.md">true</a> media_unread:flags.5?<a href="./type/true.md">true</a> silent:flags.13?<a href="./type/true.md">true</a> post:flags.14?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> from_id:flags.8?<a href="./type/int.md">int</a> to_id:<a href="./type/Peer.md">Peer</a> fwd_from:flags.2?<a href="./type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="./type/int.md">int</a> reply_to_msg_id:flags.3?<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> message:<a href="./type/string.md">string</a> media:flags.9?<a href="./type/MessageMedia.md">MessageMedia</a> reply_markup:flags.6?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.7?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; views:flags.10?<a href="./type/int.md">int</a> edit_date:flags.15?<a href="./type/int.md">int</a> = <a href="./type/Message.md">Message</a>;
<a href="./constructor/messageService.md">messageService</a>#9e19a1f6 flags:# out:flags.1?<a href="./type/true.md">true</a> mentioned:flags.4?<a href="./type/true.md">true</a> media_unread:flags.5?<a href="./type/true.md">true</a> silent:flags.13?<a href="./type/true.md">true</a> post:flags.14?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> from_id:flags.8?<a href="./type/int.md">int</a> to_id:<a href="./type/Peer.md">Peer</a> reply_to_msg_id:flags.3?<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> action:<a href="./type/MessageAction.md">MessageAction</a> = <a href="./type/Message.md">Message</a>;

<a href="./constructor/messageMediaEmpty.md">messageMediaEmpty</a>#3ded6320 = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaPhoto.md">messageMediaPhoto</a>#3d8ce53d photo:<a href="./type/Photo.md">Photo</a> caption:<a href="./type/string.md">string</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaGeo.md">messageMediaGeo</a>#56e0d474 geo:<a href="./type/GeoPoint.md">GeoPoint</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaContact.md">messageMediaContact</a>#5e7d2f39 phone_number:<a href="./type/string.md">string</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> user_id:<a href="./type/int.md">int</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaUnsupported.md">messageMediaUnsupported</a>#9f84f49e = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaDocument.md">messageMediaDocument</a>#f3e02ea8 document:<a href="./type/Document.md">Document</a> caption:<a href="./type/string.md">string</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaWebPage.md">messageMediaWebPage</a>#a32dd600 webpage:<a href="./type/WebPage.md">WebPage</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaVenue.md">messageMediaVenue</a>#7912b71f geo:<a href="./type/GeoPoint.md">GeoPoint</a> title:<a href="./type/string.md">string</a> address:<a href="./type/string.md">string</a> provider:<a href="./type/string.md">string</a> venue_id:<a href="./type/string.md">string</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaGame.md">messageMediaGame</a>#fdb19008 game:<a href="./type/Game.md">Game</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./constructor/messageMediaInvoice.md">messageMediaInvoice</a>#84551347 flags:# shipping_address_requested:flags.1?<a href="./type/true.md">true</a> test:flags.3?<a href="./type/true.md">true</a> title:<a href="./type/string.md">string</a> description:<a href="./type/string.md">string</a> photo:flags.0?<a href="./type/WebDocument.md">WebDocument</a> receipt_msg_id:flags.2?<a href="./type/int.md">int</a> currency:<a href="./type/string.md">string</a> total_amount:<a href="./type/long.md">long</a> start_param:<a href="./type/string.md">string</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;

<a href="./constructor/messageActionEmpty.md">messageActionEmpty</a>#b6aef7b0 = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatCreate.md">messageActionChatCreate</a>#a6638b9a title:<a href="./type/string.md">string</a> users:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatEditTitle.md">messageActionChatEditTitle</a>#b5a1ce5a title:<a href="./type/string.md">string</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatEditPhoto.md">messageActionChatEditPhoto</a>#7fcb13a8 photo:<a href="./type/Photo.md">Photo</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatDeletePhoto.md">messageActionChatDeletePhoto</a>#95e3fbef = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatAddUser.md">messageActionChatAddUser</a>#488a7337 users:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatDeleteUser.md">messageActionChatDeleteUser</a>#b2ae9b0c user_id:<a href="./type/int.md">int</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatJoinedByLink.md">messageActionChatJoinedByLink</a>#f89cf5e8 inviter_id:<a href="./type/int.md">int</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChannelCreate.md">messageActionChannelCreate</a>#95d2ac92 title:<a href="./type/string.md">string</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChatMigrateTo.md">messageActionChatMigrateTo</a>#51bdb021 channel_id:<a href="./type/int.md">int</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionChannelMigrateFrom.md">messageActionChannelMigrateFrom</a>#b055eaee title:<a href="./type/string.md">string</a> chat_id:<a href="./type/int.md">int</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionPinMessage.md">messageActionPinMessage</a>#94bd38ed = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionHistoryClear.md">messageActionHistoryClear</a>#9fbab604 = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionGameScore.md">messageActionGameScore</a>#92a72876 game_id:<a href="./type/long.md">long</a> score:<a href="./type/int.md">int</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionPaymentSentMe.md">messageActionPaymentSentMe</a>#8f31b327 flags:# currency:<a href="./type/string.md">string</a> total_amount:<a href="./type/long.md">long</a> payload:<a href="./type/bytes.md">bytes</a> info:flags.0?<a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> shipping_option_id:flags.1?<a href="./type/string.md">string</a> charge:<a href="./type/PaymentCharge.md">PaymentCharge</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionPaymentSent.md">messageActionPaymentSent</a>#40699cd0 currency:<a href="./type/string.md">string</a> total_amount:<a href="./type/long.md">long</a> = <a href="./type/MessageAction.md">MessageAction</a>;
<a href="./constructor/messageActionPhoneCall.md">messageActionPhoneCall</a>#80e11a7f flags:# call_id:<a href="./type/long.md">long</a> reason:flags.0?<a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a> duration:flags.1?<a href="./type/int.md">int</a> = <a href="./type/MessageAction.md">MessageAction</a>;

<a href="./constructor/dialog.md">dialog</a>#66ffba14 flags:# pinned:flags.2?<a href="./type/true.md">true</a> peer:<a href="./type/Peer.md">Peer</a> top_message:<a href="./type/int.md">int</a> read_inbox_max_id:<a href="./type/int.md">int</a> read_outbox_max_id:<a href="./type/int.md">int</a> unread_count:<a href="./type/int.md">int</a> notify_settings:<a href="./type/PeerNotifySettings.md">PeerNotifySettings</a> pts:flags.0?<a href="./type/int.md">int</a> draft:flags.1?<a href="./type/DraftMessage.md">DraftMessage</a> = <a href="./type/Dialog.md">Dialog</a>;

<a href="./constructor/photoEmpty.md">photoEmpty</a>#2331b22d id:<a href="./type/long.md">long</a> = <a href="./type/Photo.md">Photo</a>;
<a href="./constructor/photo.md">photo</a>#9288dd29 flags:# has_stickers:flags.0?<a href="./type/true.md">true</a> id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> sizes:Vector&lt;<a href="./type/PhotoSize.md">PhotoSize</a>&gt; = <a href="./type/Photo.md">Photo</a>;

<a href="./constructor/photoSizeEmpty.md">photoSizeEmpty</a>#e17e23c type:<a href="./type/string.md">string</a> = <a href="./type/PhotoSize.md">PhotoSize</a>;
<a href="./constructor/photoSize.md">photoSize</a>#77bfb61b type:<a href="./type/string.md">string</a> location:<a href="./type/FileLocation.md">FileLocation</a> w:<a href="./type/int.md">int</a> h:<a href="./type/int.md">int</a> size:<a href="./type/int.md">int</a> = <a href="./type/PhotoSize.md">PhotoSize</a>;
<a href="./constructor/photoCachedSize.md">photoCachedSize</a>#e9a734fa type:<a href="./type/string.md">string</a> location:<a href="./type/FileLocation.md">FileLocation</a> w:<a href="./type/int.md">int</a> h:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/PhotoSize.md">PhotoSize</a>;

<a href="./constructor/geoPointEmpty.md">geoPointEmpty</a>#1117dd5f = <a href="./type/GeoPoint.md">GeoPoint</a>;
<a href="./constructor/geoPoint.md">geoPoint</a>#2049d70c long:<a href="./type/double.md">double</a> lat:<a href="./type/double.md">double</a> = <a href="./type/GeoPoint.md">GeoPoint</a>;

<a href="./constructor/auth.checkedPhone.md">auth.checkedPhone</a>#811ea28e phone_registered:<a href="./type/Bool.md">Bool</a> = <a href="./type/auth.CheckedPhone.md">auth.CheckedPhone</a>;

<a href="./constructor/auth.sentCode.md">auth.sentCode</a>#5e002502 flags:# phone_registered:flags.0?<a href="./type/true.md">true</a> type:<a href="./type/auth.SentCodeType.md">auth.SentCodeType</a> phone_code_hash:<a href="./type/string.md">string</a> next_type:flags.1?<a href="./type/auth.CodeType.md">auth.CodeType</a> timeout:flags.2?<a href="./type/int.md">int</a> = <a href="./type/auth.SentCode.md">auth.SentCode</a>;

<a href="./constructor/auth.authorization.md">auth.authorization</a>#cd050916 flags:# tmp_sessions:flags.0?<a href="./type/int.md">int</a> user:<a href="./type/User.md">User</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;

<a href="./constructor/auth.exportedAuthorization.md">auth.exportedAuthorization</a>#df969c2d id:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/auth.ExportedAuthorization.md">auth.ExportedAuthorization</a>;

<a href="./constructor/inputNotifyPeer.md">inputNotifyPeer</a>#b8bc5b0c peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/InputNotifyPeer.md">InputNotifyPeer</a>;
<a href="./constructor/inputNotifyUsers.md">inputNotifyUsers</a>#193b4417 = <a href="./type/InputNotifyPeer.md">InputNotifyPeer</a>;
<a href="./constructor/inputNotifyChats.md">inputNotifyChats</a>#4a95e84e = <a href="./type/InputNotifyPeer.md">InputNotifyPeer</a>;
<a href="./constructor/inputNotifyAll.md">inputNotifyAll</a>#a429b886 = <a href="./type/InputNotifyPeer.md">InputNotifyPeer</a>;

<a href="./constructor/inputPeerNotifyEventsEmpty.md">inputPeerNotifyEventsEmpty</a>#f03064d8 = <a href="./type/InputPeerNotifyEvents.md">InputPeerNotifyEvents</a>;
<a href="./constructor/inputPeerNotifyEventsAll.md">inputPeerNotifyEventsAll</a>#e86a2c74 = <a href="./type/InputPeerNotifyEvents.md">InputPeerNotifyEvents</a>;

<a href="./constructor/inputPeerNotifySettings.md">inputPeerNotifySettings</a>#38935eb2 flags:# show_previews:flags.0?<a href="./type/true.md">true</a> silent:flags.1?<a href="./type/true.md">true</a> mute_until:<a href="./type/int.md">int</a> sound:<a href="./type/string.md">string</a> = <a href="./type/InputPeerNotifySettings.md">InputPeerNotifySettings</a>;

<a href="./constructor/peerNotifyEventsEmpty.md">peerNotifyEventsEmpty</a>#add53cb3 = <a href="./type/PeerNotifyEvents.md">PeerNotifyEvents</a>;
<a href="./constructor/peerNotifyEventsAll.md">peerNotifyEventsAll</a>#6d1ded88 = <a href="./type/PeerNotifyEvents.md">PeerNotifyEvents</a>;

<a href="./constructor/peerNotifySettingsEmpty.md">peerNotifySettingsEmpty</a>#70a68512 = <a href="./type/PeerNotifySettings.md">PeerNotifySettings</a>;
<a href="./constructor/peerNotifySettings.md">peerNotifySettings</a>#9acda4c0 flags:# show_previews:flags.0?<a href="./type/true.md">true</a> silent:flags.1?<a href="./type/true.md">true</a> mute_until:<a href="./type/int.md">int</a> sound:<a href="./type/string.md">string</a> = <a href="./type/PeerNotifySettings.md">PeerNotifySettings</a>;

<a href="./constructor/peerSettings.md">peerSettings</a>#818426cd flags:# report_spam:flags.0?<a href="./type/true.md">true</a> = <a href="./type/PeerSettings.md">PeerSettings</a>;

<a href="./constructor/wallPaper.md">wallPaper</a>#ccb03657 id:<a href="./type/int.md">int</a> title:<a href="./type/string.md">string</a> sizes:Vector&lt;<a href="./type/PhotoSize.md">PhotoSize</a>&gt; color:<a href="./type/int.md">int</a> = <a href="./type/WallPaper.md">WallPaper</a>;
<a href="./constructor/wallPaperSolid.md">wallPaperSolid</a>#63117f24 id:<a href="./type/int.md">int</a> title:<a href="./type/string.md">string</a> bg_color:<a href="./type/int.md">int</a> color:<a href="./type/int.md">int</a> = <a href="./type/WallPaper.md">WallPaper</a>;

<a href="./constructor/inputReportReasonSpam.md">inputReportReasonSpam</a>#58dbcab8 = <a href="./type/ReportReason.md">ReportReason</a>;
<a href="./constructor/inputReportReasonViolence.md">inputReportReasonViolence</a>#1e22c78d = <a href="./type/ReportReason.md">ReportReason</a>;
<a href="./constructor/inputReportReasonPornography.md">inputReportReasonPornography</a>#2e59d922 = <a href="./type/ReportReason.md">ReportReason</a>;
<a href="./constructor/inputReportReasonOther.md">inputReportReasonOther</a>#e1746d0a text:<a href="./type/string.md">string</a> = <a href="./type/ReportReason.md">ReportReason</a>;

<a href="./constructor/userFull.md">userFull</a>#f220f3f flags:# blocked:flags.0?<a href="./type/true.md">true</a> phone_calls_available:flags.4?<a href="./type/true.md">true</a> phone_calls_private:flags.5?<a href="./type/true.md">true</a> user:<a href="./type/User.md">User</a> about:flags.1?<a href="./type/string.md">string</a> link:<a href="./type/contacts.Link.md">contacts.Link</a> profile_photo:flags.2?<a href="./type/Photo.md">Photo</a> notify_settings:<a href="./type/PeerNotifySettings.md">PeerNotifySettings</a> bot_info:flags.3?<a href="./type/BotInfo.md">BotInfo</a> common_chats_count:<a href="./type/int.md">int</a> = <a href="./type/UserFull.md">UserFull</a>;

<a href="./constructor/contact.md">contact</a>#f911c994 user_id:<a href="./type/int.md">int</a> mutual:<a href="./type/Bool.md">Bool</a> = <a href="./type/Contact.md">Contact</a>;

<a href="./constructor/importedContact.md">importedContact</a>#d0028438 user_id:<a href="./type/int.md">int</a> client_id:<a href="./type/long.md">long</a> = <a href="./type/ImportedContact.md">ImportedContact</a>;

<a href="./constructor/contactBlocked.md">contactBlocked</a>#561bc879 user_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ContactBlocked.md">ContactBlocked</a>;

<a href="./constructor/contactStatus.md">contactStatus</a>#d3680c61 user_id:<a href="./type/int.md">int</a> status:<a href="./type/UserStatus.md">UserStatus</a> = <a href="./type/ContactStatus.md">ContactStatus</a>;

<a href="./constructor/contacts.link.md">contacts.link</a>#3ace484c my_link:<a href="./type/ContactLink.md">ContactLink</a> foreign_link:<a href="./type/ContactLink.md">ContactLink</a> user:<a href="./type/User.md">User</a> = <a href="./type/contacts.Link.md">contacts.Link</a>;

<a href="./constructor/contacts.contactsNotModified.md">contacts.contactsNotModified</a>#b74ba9d2 = <a href="./type/contacts.Contacts.md">contacts.Contacts</a>;
<a href="./constructor/contacts.contacts.md">contacts.contacts</a>#6f8b8cb2 contacts:Vector&lt;<a href="./type/Contact.md">Contact</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.Contacts.md">contacts.Contacts</a>;

<a href="./constructor/contacts.importedContacts.md">contacts.importedContacts</a>#ad524315 imported:Vector&lt;<a href="./type/ImportedContact.md">ImportedContact</a>&gt; retry_contacts:Vector&lt;<a href="./type/long.md">long</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.ImportedContacts.md">contacts.ImportedContacts</a>;

<a href="./constructor/contacts.blocked.md">contacts.blocked</a>#1c138d15 blocked:Vector&lt;<a href="./type/ContactBlocked.md">ContactBlocked</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.Blocked.md">contacts.Blocked</a>;
<a href="./constructor/contacts.blockedSlice.md">contacts.blockedSlice</a>#900802a1 count:<a href="./type/int.md">int</a> blocked:Vector&lt;<a href="./type/ContactBlocked.md">ContactBlocked</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.Blocked.md">contacts.Blocked</a>;

<a href="./constructor/messages.dialogs.md">messages.dialogs</a>#15ba6c40 dialogs:Vector&lt;<a href="./type/Dialog.md">Dialog</a>&gt; messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.Dialogs.md">messages.Dialogs</a>;
<a href="./constructor/messages.dialogsSlice.md">messages.dialogsSlice</a>#71e094f3 count:<a href="./type/int.md">int</a> dialogs:Vector&lt;<a href="./type/Dialog.md">Dialog</a>&gt; messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.Dialogs.md">messages.Dialogs</a>;

<a href="./constructor/messages.messages.md">messages.messages</a>#8c718e87 messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./constructor/messages.messagesSlice.md">messages.messagesSlice</a>#b446ae3 count:<a href="./type/int.md">int</a> messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./constructor/messages.channelMessages.md">messages.channelMessages</a>#99262e37 flags:# pts:<a href="./type/int.md">int</a> count:<a href="./type/int.md">int</a> messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.Messages.md">messages.Messages</a>;

<a href="./constructor/messages.chats.md">messages.chats</a>#64ff9fd5 chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; = <a href="./type/messages.Chats.md">messages.Chats</a>;
<a href="./constructor/messages.chatsSlice.md">messages.chatsSlice</a>#9cd81144 count:<a href="./type/int.md">int</a> chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; = <a href="./type/messages.Chats.md">messages.Chats</a>;

<a href="./constructor/messages.chatFull.md">messages.chatFull</a>#e5d7d19c full_chat:<a href="./type/ChatFull.md">ChatFull</a> chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.ChatFull.md">messages.ChatFull</a>;

<a href="./constructor/messages.affectedHistory.md">messages.affectedHistory</a>#b45c69d1 pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> offset:<a href="./type/int.md">int</a> = <a href="./type/messages.AffectedHistory.md">messages.AffectedHistory</a>;

<a href="./constructor/inputMessagesFilterEmpty.md">inputMessagesFilterEmpty</a>#57e2f66c = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterPhotos.md">inputMessagesFilterPhotos</a>#9609a51c = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterVideo.md">inputMessagesFilterVideo</a>#9fc00e65 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterPhotoVideo.md">inputMessagesFilterPhotoVideo</a>#56e9f0e4 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterPhotoVideoDocuments.md">inputMessagesFilterPhotoVideoDocuments</a>#d95e73bb = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterDocument.md">inputMessagesFilterDocument</a>#9eddf188 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterUrl.md">inputMessagesFilterUrl</a>#7ef0dd87 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterGif.md">inputMessagesFilterGif</a>#ffc86587 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterVoice.md">inputMessagesFilterVoice</a>#50f5c392 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterMusic.md">inputMessagesFilterMusic</a>#3751b49e = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterChatPhotos.md">inputMessagesFilterChatPhotos</a>#3a20ecb8 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterPhoneCalls.md">inputMessagesFilterPhoneCalls</a>#80c99768 flags:# missed:flags.0?<a href="./type/true.md">true</a> = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterRoundVoice.md">inputMessagesFilterRoundVoice</a>#7a7c17a4 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;
<a href="./constructor/inputMessagesFilterRoundVideo.md">inputMessagesFilterRoundVideo</a>#b549da53 = <a href="./type/MessagesFilter.md">MessagesFilter</a>;

<a href="./constructor/updateNewMessage.md">updateNewMessage</a>#1f2b0afd message:<a href="./type/Message.md">Message</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateMessageID.md">updateMessageID</a>#4e90bfd6 id:<a href="./type/int.md">int</a> random_id:<a href="./type/long.md">long</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateDeleteMessages.md">updateDeleteMessages</a>#a20db0e5 messages:Vector&lt;<a href="./type/int.md">int</a>&gt; pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateUserTyping.md">updateUserTyping</a>#5c486927 user_id:<a href="./type/int.md">int</a> action:<a href="./type/SendMessageAction.md">SendMessageAction</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChatUserTyping.md">updateChatUserTyping</a>#9a65ea1f chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> action:<a href="./type/SendMessageAction.md">SendMessageAction</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChatParticipants.md">updateChatParticipants</a>#7761198 participants:<a href="./type/ChatParticipants.md">ChatParticipants</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateUserStatus.md">updateUserStatus</a>#1bfbd823 user_id:<a href="./type/int.md">int</a> status:<a href="./type/UserStatus.md">UserStatus</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateUserName.md">updateUserName</a>#a7332b73 user_id:<a href="./type/int.md">int</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> username:<a href="./type/string.md">string</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateUserPhoto.md">updateUserPhoto</a>#95313b0c user_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> photo:<a href="./type/UserProfilePhoto.md">UserProfilePhoto</a> previous:<a href="./type/Bool.md">Bool</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateContactRegistered.md">updateContactRegistered</a>#2575bbb9 user_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateContactLink.md">updateContactLink</a>#9d2e67c5 user_id:<a href="./type/int.md">int</a> my_link:<a href="./type/ContactLink.md">ContactLink</a> foreign_link:<a href="./type/ContactLink.md">ContactLink</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateNewEncryptedMessage.md">updateNewEncryptedMessage</a>#12bcbd9a message:<a href="./type/EncryptedMessage.md">EncryptedMessage</a> qts:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateEncryptedChatTyping.md">updateEncryptedChatTyping</a>#1710f156 chat_id:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateEncryption.md">updateEncryption</a>#b4a2e88d chat:<a href="./type/EncryptedChat.md">EncryptedChat</a> date:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateEncryptedMessagesRead.md">updateEncryptedMessagesRead</a>#38fe25b7 chat_id:<a href="./type/int.md">int</a> max_date:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChatParticipantAdd.md">updateChatParticipantAdd</a>#ea4b0e5c chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> inviter_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> version:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChatParticipantDelete.md">updateChatParticipantDelete</a>#6e5f8c22 chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> version:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateDcOptions.md">updateDcOptions</a>#8e5e9873 dc_options:Vector&lt;<a href="./type/DcOption.md">DcOption</a>&gt; = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateUserBlocked.md">updateUserBlocked</a>#80ece81a user_id:<a href="./type/int.md">int</a> blocked:<a href="./type/Bool.md">Bool</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateNotifySettings.md">updateNotifySettings</a>#bec268ef peer:<a href="./type/NotifyPeer.md">NotifyPeer</a> notify_settings:<a href="./type/PeerNotifySettings.md">PeerNotifySettings</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateServiceNotification.md">updateServiceNotification</a>#ebe46819 flags:# popup:flags.0?<a href="./type/true.md">true</a> inbox_date:flags.1?<a href="./type/int.md">int</a> type:<a href="./type/string.md">string</a> message:<a href="./type/string.md">string</a> media:<a href="./type/MessageMedia.md">MessageMedia</a> entities:Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updatePrivacy.md">updatePrivacy</a>#ee3b272a key:<a href="./type/PrivacyKey.md">PrivacyKey</a> rules:Vector&lt;<a href="./type/PrivacyRule.md">PrivacyRule</a>&gt; = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateUserPhone.md">updateUserPhone</a>#12b9417b user_id:<a href="./type/int.md">int</a> phone:<a href="./type/string.md">string</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateReadHistoryInbox.md">updateReadHistoryInbox</a>#9961fd5c peer:<a href="./type/Peer.md">Peer</a> max_id:<a href="./type/int.md">int</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateReadHistoryOutbox.md">updateReadHistoryOutbox</a>#2f2f21bf peer:<a href="./type/Peer.md">Peer</a> max_id:<a href="./type/int.md">int</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateWebPage.md">updateWebPage</a>#7f891213 webpage:<a href="./type/WebPage.md">WebPage</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateReadMessagesContents.md">updateReadMessagesContents</a>#68c13933 messages:Vector&lt;<a href="./type/int.md">int</a>&gt; pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChannelTooLong.md">updateChannelTooLong</a>#eb0467fb flags:# channel_id:<a href="./type/int.md">int</a> pts:flags.0?<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChannel.md">updateChannel</a>#b6d45656 channel_id:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateNewChannelMessage.md">updateNewChannelMessage</a>#62ba04d9 message:<a href="./type/Message.md">Message</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateReadChannelInbox.md">updateReadChannelInbox</a>#4214f37f channel_id:<a href="./type/int.md">int</a> max_id:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateDeleteChannelMessages.md">updateDeleteChannelMessages</a>#c37521c9 channel_id:<a href="./type/int.md">int</a> messages:Vector&lt;<a href="./type/int.md">int</a>&gt; pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChannelMessageViews.md">updateChannelMessageViews</a>#98a12b4b channel_id:<a href="./type/int.md">int</a> id:<a href="./type/int.md">int</a> views:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChatAdmins.md">updateChatAdmins</a>#6e947941 chat_id:<a href="./type/int.md">int</a> enabled:<a href="./type/Bool.md">Bool</a> version:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChatParticipantAdmin.md">updateChatParticipantAdmin</a>#b6901959 chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> is_admin:<a href="./type/Bool.md">Bool</a> version:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateNewStickerSet.md">updateNewStickerSet</a>#688a30aa stickerset:<a href="./type/messages.StickerSet.md">messages.StickerSet</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateStickerSetsOrder.md">updateStickerSetsOrder</a>#bb2d201 flags:# masks:flags.0?<a href="./type/true.md">true</a> order:Vector&lt;<a href="./type/long.md">long</a>&gt; = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateStickerSets.md">updateStickerSets</a>#43ae3dec = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateSavedGifs.md">updateSavedGifs</a>#9375341e = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotInlineQuery.md">updateBotInlineQuery</a>#54826690 flags:# query_id:<a href="./type/long.md">long</a> user_id:<a href="./type/int.md">int</a> query:<a href="./type/string.md">string</a> geo:flags.0?<a href="./type/GeoPoint.md">GeoPoint</a> offset:<a href="./type/string.md">string</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotInlineSend.md">updateBotInlineSend</a>#e48f964 flags:# user_id:<a href="./type/int.md">int</a> query:<a href="./type/string.md">string</a> geo:flags.0?<a href="./type/GeoPoint.md">GeoPoint</a> id:<a href="./type/string.md">string</a> msg_id:flags.1?<a href="./type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateEditChannelMessage.md">updateEditChannelMessage</a>#1b3f4df7 message:<a href="./type/Message.md">Message</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChannelPinnedMessage.md">updateChannelPinnedMessage</a>#98592475 channel_id:<a href="./type/int.md">int</a> id:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotCallbackQuery.md">updateBotCallbackQuery</a>#e73547e1 flags:# query_id:<a href="./type/long.md">long</a> user_id:<a href="./type/int.md">int</a> peer:<a href="./type/Peer.md">Peer</a> msg_id:<a href="./type/int.md">int</a> chat_instance:<a href="./type/long.md">long</a> data:flags.0?<a href="./type/bytes.md">bytes</a> game_short_name:flags.1?<a href="./type/string.md">string</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateEditMessage.md">updateEditMessage</a>#e40370a3 message:<a href="./type/Message.md">Message</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateInlineBotCallbackQuery.md">updateInlineBotCallbackQuery</a>#f9d27a5a flags:# query_id:<a href="./type/long.md">long</a> user_id:<a href="./type/int.md">int</a> msg_id:<a href="./type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> chat_instance:<a href="./type/long.md">long</a> data:flags.0?<a href="./type/bytes.md">bytes</a> game_short_name:flags.1?<a href="./type/string.md">string</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateReadChannelOutbox.md">updateReadChannelOutbox</a>#25d6c9c7 channel_id:<a href="./type/int.md">int</a> max_id:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateDraftMessage.md">updateDraftMessage</a>#ee2bb969 peer:<a href="./type/Peer.md">Peer</a> draft:<a href="./type/DraftMessage.md">DraftMessage</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateReadFeaturedStickers.md">updateReadFeaturedStickers</a>#571d2742 = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateRecentStickers.md">updateRecentStickers</a>#9a422c20 = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateConfig.md">updateConfig</a>#a229dd06 = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updatePtsChanged.md">updatePtsChanged</a>#3354678f = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateChannelWebPage.md">updateChannelWebPage</a>#40771900 channel_id:<a href="./type/int.md">int</a> webpage:<a href="./type/WebPage.md">WebPage</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateDialogPinned.md">updateDialogPinned</a>#d711a2cc flags:# pinned:flags.0?<a href="./type/true.md">true</a> peer:<a href="./type/Peer.md">Peer</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updatePinnedDialogs.md">updatePinnedDialogs</a>#d8caf68d flags:# order:flags.0?Vector&lt;<a href="./type/Peer.md">Peer</a>&gt; = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotWebhookJSON.md">updateBotWebhookJSON</a>#8317c0c3 data:<a href="./type/DataJSON.md">DataJSON</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotWebhookJSONQuery.md">updateBotWebhookJSONQuery</a>#9b9240a6 query_id:<a href="./type/long.md">long</a> data:<a href="./type/DataJSON.md">DataJSON</a> timeout:<a href="./type/int.md">int</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotShippingQuery.md">updateBotShippingQuery</a>#e0cdc940 query_id:<a href="./type/long.md">long</a> user_id:<a href="./type/int.md">int</a> payload:<a href="./type/bytes.md">bytes</a> shipping_address:<a href="./type/PostAddress.md">PostAddress</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updateBotPrecheckoutQuery.md">updateBotPrecheckoutQuery</a>#5d2f3aa9 flags:# query_id:<a href="./type/long.md">long</a> user_id:<a href="./type/int.md">int</a> payload:<a href="./type/bytes.md">bytes</a> info:flags.0?<a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> shipping_option_id:flags.1?<a href="./type/string.md">string</a> currency:<a href="./type/string.md">string</a> total_amount:<a href="./type/long.md">long</a> = <a href="./type/Update.md">Update</a>;
<a href="./constructor/updatePhoneCall.md">updatePhoneCall</a>#ab0f6b1e phone_call:<a href="./type/PhoneCall.md">PhoneCall</a> = <a href="./type/Update.md">Update</a>;

<a href="./constructor/updates.state.md">updates.state</a>#a56c2a3e pts:<a href="./type/int.md">int</a> qts:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> seq:<a href="./type/int.md">int</a> unread_count:<a href="./type/int.md">int</a> = <a href="./type/updates.State.md">updates.State</a>;

<a href="./constructor/updates.differenceEmpty.md">updates.differenceEmpty</a>#5d75a138 date:<a href="./type/int.md">int</a> seq:<a href="./type/int.md">int</a> = <a href="./type/updates.Difference.md">updates.Difference</a>;
<a href="./constructor/updates.difference.md">updates.difference</a>#f49ca0 new_messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; new_encrypted_messages:Vector&lt;<a href="./type/EncryptedMessage.md">EncryptedMessage</a>&gt; other_updates:Vector&lt;<a href="./type/Update.md">Update</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; state:<a href="./type/updates.State.md">updates.State</a> = <a href="./type/updates.Difference.md">updates.Difference</a>;
<a href="./constructor/updates.differenceSlice.md">updates.differenceSlice</a>#a8fb1981 new_messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; new_encrypted_messages:Vector&lt;<a href="./type/EncryptedMessage.md">EncryptedMessage</a>&gt; other_updates:Vector&lt;<a href="./type/Update.md">Update</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; intermediate_state:<a href="./type/updates.State.md">updates.State</a> = <a href="./type/updates.Difference.md">updates.Difference</a>;
<a href="./constructor/updates.differenceTooLong.md">updates.differenceTooLong</a>#4afe8f6d pts:<a href="./type/int.md">int</a> = <a href="./type/updates.Difference.md">updates.Difference</a>;

<a href="./constructor/updatesTooLong.md">updatesTooLong</a>#e317af7e = <a href="./type/Updates.md">Updates</a>;
<a href="./constructor/updateShortMessage.md">updateShortMessage</a>#914fbf11 flags:# out:flags.1?<a href="./type/true.md">true</a> mentioned:flags.4?<a href="./type/true.md">true</a> media_unread:flags.5?<a href="./type/true.md">true</a> silent:flags.13?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> message:<a href="./type/string.md">string</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> fwd_from:flags.2?<a href="./type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="./type/int.md">int</a> reply_to_msg_id:flags.3?<a href="./type/int.md">int</a> entities:flags.7?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Updates.md">Updates</a>;
<a href="./constructor/updateShortChatMessage.md">updateShortChatMessage</a>#16812688 flags:# out:flags.1?<a href="./type/true.md">true</a> mentioned:flags.4?<a href="./type/true.md">true</a> media_unread:flags.5?<a href="./type/true.md">true</a> silent:flags.13?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> from_id:<a href="./type/int.md">int</a> chat_id:<a href="./type/int.md">int</a> message:<a href="./type/string.md">string</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> fwd_from:flags.2?<a href="./type/MessageFwdHeader.md">MessageFwdHeader</a> via_bot_id:flags.11?<a href="./type/int.md">int</a> reply_to_msg_id:flags.3?<a href="./type/int.md">int</a> entities:flags.7?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Updates.md">Updates</a>;
<a href="./constructor/updateShort.md">updateShort</a>#78d4dec1 update:<a href="./type/Update.md">Update</a> date:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./constructor/updatesCombined.md">updatesCombined</a>#725b04c3 updates:Vector&lt;<a href="./type/Update.md">Update</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; date:<a href="./type/int.md">int</a> seq_start:<a href="./type/int.md">int</a> seq:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./constructor/updates.md">updates</a>#74ae4240 updates:Vector&lt;<a href="./type/Update.md">Update</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; date:<a href="./type/int.md">int</a> seq:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./constructor/updateShortSentMessage.md">updateShortSentMessage</a>#11f1331c flags:# out:flags.1?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> media:flags.9?<a href="./type/MessageMedia.md">MessageMedia</a> entities:flags.7?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Updates.md">Updates</a>;

<a href="./constructor/photos.photos.md">photos.photos</a>#8dca6aa5 photos:Vector&lt;<a href="./type/Photo.md">Photo</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/photos.Photos.md">photos.Photos</a>;
<a href="./constructor/photos.photosSlice.md">photos.photosSlice</a>#15051f54 count:<a href="./type/int.md">int</a> photos:Vector&lt;<a href="./type/Photo.md">Photo</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/photos.Photos.md">photos.Photos</a>;

<a href="./constructor/photos.photo.md">photos.photo</a>#20212ca8 photo:<a href="./type/Photo.md">Photo</a> users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/photos.Photo.md">photos.Photo</a>;

<a href="./constructor/upload.file.md">upload.file</a>#96a18d5 type:<a href="./type/storage.FileType.md">storage.FileType</a> mtime:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/upload.File.md">upload.File</a>;
<a href="./constructor/upload.fileCdnRedirect.md">upload.fileCdnRedirect</a>#1508485a dc_id:<a href="./type/int.md">int</a> file_token:<a href="./type/bytes.md">bytes</a> encryption_key:<a href="./type/bytes.md">bytes</a> encryption_iv:<a href="./type/bytes.md">bytes</a> = <a href="./type/upload.File.md">upload.File</a>;

<a href="./constructor/dcOption.md">dcOption</a>#5d8c6cc flags:# ipv6:flags.0?<a href="./type/true.md">true</a> media_only:flags.1?<a href="./type/true.md">true</a> tcpo_only:flags.2?<a href="./type/true.md">true</a> cdn:flags.3?<a href="./type/true.md">true</a> id:<a href="./type/int.md">int</a> ip_address:<a href="./type/string.md">string</a> port:<a href="./type/int.md">int</a> = <a href="./type/DcOption.md">DcOption</a>;

<a href="./constructor/config.md">config</a>#cb601684 flags:# phonecalls_enabled:flags.1?<a href="./type/true.md">true</a> date:<a href="./type/int.md">int</a> expires:<a href="./type/int.md">int</a> test_mode:<a href="./type/Bool.md">Bool</a> this_dc:<a href="./type/int.md">int</a> dc_options:Vector&lt;<a href="./type/DcOption.md">DcOption</a>&gt; chat_size_max:<a href="./type/int.md">int</a> megagroup_size_max:<a href="./type/int.md">int</a> forwarded_count_max:<a href="./type/int.md">int</a> online_update_period_ms:<a href="./type/int.md">int</a> offline_blur_timeout_ms:<a href="./type/int.md">int</a> offline_idle_timeout_ms:<a href="./type/int.md">int</a> online_cloud_timeout_ms:<a href="./type/int.md">int</a> notify_cloud_delay_ms:<a href="./type/int.md">int</a> notify_default_delay_ms:<a href="./type/int.md">int</a> chat_big_size:<a href="./type/int.md">int</a> push_chat_period_ms:<a href="./type/int.md">int</a> push_chat_limit:<a href="./type/int.md">int</a> saved_gifs_limit:<a href="./type/int.md">int</a> edit_time_limit:<a href="./type/int.md">int</a> rating_e_decay:<a href="./type/int.md">int</a> stickers_recent_limit:<a href="./type/int.md">int</a> tmp_sessions:flags.0?<a href="./type/int.md">int</a> pinned_dialogs_count_max:<a href="./type/int.md">int</a> call_receive_timeout_ms:<a href="./type/int.md">int</a> call_ring_timeout_ms:<a href="./type/int.md">int</a> call_connect_timeout_ms:<a href="./type/int.md">int</a> call_packet_timeout_ms:<a href="./type/int.md">int</a> me_url_prefix:<a href="./type/string.md">string</a> disabled_features:Vector&lt;<a href="./type/DisabledFeature.md">DisabledFeature</a>&gt; = <a href="./type/Config.md">Config</a>;

<a href="./constructor/nearestDc.md">nearestDc</a>#8e1a1775 country:<a href="./type/string.md">string</a> this_dc:<a href="./type/int.md">int</a> nearest_dc:<a href="./type/int.md">int</a> = <a href="./type/NearestDc.md">NearestDc</a>;

<a href="./constructor/help.appUpdate.md">help.appUpdate</a>#8987f311 id:<a href="./type/int.md">int</a> critical:<a href="./type/Bool.md">Bool</a> url:<a href="./type/string.md">string</a> text:<a href="./type/string.md">string</a> = <a href="./type/help.AppUpdate.md">help.AppUpdate</a>;
<a href="./constructor/help.noAppUpdate.md">help.noAppUpdate</a>#c45a6536 = <a href="./type/help.AppUpdate.md">help.AppUpdate</a>;

<a href="./constructor/help.inviteText.md">help.inviteText</a>#18cb9f78 message:<a href="./type/string.md">string</a> = <a href="./type/help.InviteText.md">help.InviteText</a>;

<a href="./constructor/encryptedChatEmpty.md">encryptedChatEmpty</a>#ab7ec0a0 id:<a href="./type/int.md">int</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;
<a href="./constructor/encryptedChatWaiting.md">encryptedChatWaiting</a>#3bf703dc id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;
<a href="./constructor/encryptedChatRequested.md">encryptedChatRequested</a>#c878527e id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> g_a:<a href="./type/bytes.md">bytes</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;
<a href="./constructor/encryptedChat.md">encryptedChat</a>#fa56ce36 id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> g_a_or_b:<a href="./type/bytes.md">bytes</a> key_fingerprint:<a href="./type/long.md">long</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;
<a href="./constructor/encryptedChatDiscarded.md">encryptedChatDiscarded</a>#13d6dd27 id:<a href="./type/int.md">int</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;

<a href="./constructor/inputEncryptedChat.md">inputEncryptedChat</a>#f141b5e1 chat_id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputEncryptedChat.md">InputEncryptedChat</a>;

<a href="./constructor/encryptedFileEmpty.md">encryptedFileEmpty</a>#c21f497e = <a href="./type/EncryptedFile.md">EncryptedFile</a>;
<a href="./constructor/encryptedFile.md">encryptedFile</a>#4a70994c id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> size:<a href="./type/int.md">int</a> dc_id:<a href="./type/int.md">int</a> key_fingerprint:<a href="./type/int.md">int</a> = <a href="./type/EncryptedFile.md">EncryptedFile</a>;

<a href="./constructor/inputEncryptedFileEmpty.md">inputEncryptedFileEmpty</a>#1837c364 = <a href="./type/InputEncryptedFile.md">InputEncryptedFile</a>;
<a href="./constructor/inputEncryptedFileUploaded.md">inputEncryptedFileUploaded</a>#64bd0306 id:<a href="./type/long.md">long</a> parts:<a href="./type/int.md">int</a> md5_checksum:<a href="./type/string.md">string</a> key_fingerprint:<a href="./type/int.md">int</a> = <a href="./type/InputEncryptedFile.md">InputEncryptedFile</a>;
<a href="./constructor/inputEncryptedFile.md">inputEncryptedFile</a>#5a17b5e5 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputEncryptedFile.md">InputEncryptedFile</a>;
<a href="./constructor/inputEncryptedFileBigUploaded.md">inputEncryptedFileBigUploaded</a>#2dc173c8 id:<a href="./type/long.md">long</a> parts:<a href="./type/int.md">int</a> key_fingerprint:<a href="./type/int.md">int</a> = <a href="./type/InputEncryptedFile.md">InputEncryptedFile</a>;

<a href="./constructor/encryptedMessage.md">encryptedMessage</a>#ed18c118 random_id:<a href="./type/long.md">long</a> chat_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> file:<a href="./type/EncryptedFile.md">EncryptedFile</a> = <a href="./type/EncryptedMessage.md">EncryptedMessage</a>;
<a href="./constructor/encryptedMessageService.md">encryptedMessageService</a>#23734b06 random_id:<a href="./type/long.md">long</a> chat_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/EncryptedMessage.md">EncryptedMessage</a>;

<a href="./constructor/messages.dhConfigNotModified.md">messages.dhConfigNotModified</a>#c0e24635 random:<a href="./type/bytes.md">bytes</a> = <a href="./type/messages.DhConfig.md">messages.DhConfig</a>;
<a href="./constructor/messages.dhConfig.md">messages.dhConfig</a>#2c221edd g:<a href="./type/int.md">int</a> p:<a href="./type/bytes.md">bytes</a> version:<a href="./type/int.md">int</a> random:<a href="./type/bytes.md">bytes</a> = <a href="./type/messages.DhConfig.md">messages.DhConfig</a>;

<a href="./constructor/messages.sentEncryptedMessage.md">messages.sentEncryptedMessage</a>#560f8935 date:<a href="./type/int.md">int</a> = <a href="./type/messages.SentEncryptedMessage.md">messages.SentEncryptedMessage</a>;
<a href="./constructor/messages.sentEncryptedFile.md">messages.sentEncryptedFile</a>#9493ff32 date:<a href="./type/int.md">int</a> file:<a href="./type/EncryptedFile.md">EncryptedFile</a> = <a href="./type/messages.SentEncryptedMessage.md">messages.SentEncryptedMessage</a>;

<a href="./constructor/inputDocumentEmpty.md">inputDocumentEmpty</a>#72f0eaae = <a href="./type/InputDocument.md">InputDocument</a>;
<a href="./constructor/inputDocument.md">inputDocument</a>#18798952 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputDocument.md">InputDocument</a>;

<a href="./constructor/documentEmpty.md">documentEmpty</a>#36f8c871 id:<a href="./type/long.md">long</a> = <a href="./type/Document.md">Document</a>;
<a href="./constructor/document.md">document</a>#87232bc7 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> mime_type:<a href="./type/string.md">string</a> size:<a href="./type/int.md">int</a> thumb:<a href="./type/PhotoSize.md">PhotoSize</a> dc_id:<a href="./type/int.md">int</a> version:<a href="./type/int.md">int</a> attributes:Vector&lt;<a href="./type/DocumentAttribute.md">DocumentAttribute</a>&gt; = <a href="./type/Document.md">Document</a>;

<a href="./constructor/help.support.md">help.support</a>#17c6b5f6 phone_number:<a href="./type/string.md">string</a> user:<a href="./type/User.md">User</a> = <a href="./type/help.Support.md">help.Support</a>;

<a href="./constructor/notifyPeer.md">notifyPeer</a>#9fd40bd8 peer:<a href="./type/Peer.md">Peer</a> = <a href="./type/NotifyPeer.md">NotifyPeer</a>;
<a href="./constructor/notifyUsers.md">notifyUsers</a>#b4c83b4c = <a href="./type/NotifyPeer.md">NotifyPeer</a>;
<a href="./constructor/notifyChats.md">notifyChats</a>#c007cec3 = <a href="./type/NotifyPeer.md">NotifyPeer</a>;
<a href="./constructor/notifyAll.md">notifyAll</a>#74d07c60 = <a href="./type/NotifyPeer.md">NotifyPeer</a>;

<a href="./constructor/sendMessageTypingAction.md">sendMessageTypingAction</a>#16bf744e = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageCancelAction.md">sendMessageCancelAction</a>#fd5ec8f5 = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageRecordVideoAction.md">sendMessageRecordVideoAction</a>#a187d66f = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageUploadVideoAction.md">sendMessageUploadVideoAction</a>#e9763aec progress:<a href="./type/int.md">int</a> = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageRecordAudioAction.md">sendMessageRecordAudioAction</a>#d52f73f7 = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageUploadAudioAction.md">sendMessageUploadAudioAction</a>#f351d7ab progress:<a href="./type/int.md">int</a> = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageUploadPhotoAction.md">sendMessageUploadPhotoAction</a>#d1d34a26 progress:<a href="./type/int.md">int</a> = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageUploadDocumentAction.md">sendMessageUploadDocumentAction</a>#aa0cd9e4 progress:<a href="./type/int.md">int</a> = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageGeoLocationAction.md">sendMessageGeoLocationAction</a>#176f8ba1 = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageChooseContactAction.md">sendMessageChooseContactAction</a>#628cbc6f = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageGamePlayAction.md">sendMessageGamePlayAction</a>#dd6a8f48 = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageRecordRoundAction.md">sendMessageRecordRoundAction</a>#88f27fbc = <a href="./type/SendMessageAction.md">SendMessageAction</a>;
<a href="./constructor/sendMessageUploadRoundAction.md">sendMessageUploadRoundAction</a>#243e1c66 progress:<a href="./type/int.md">int</a> = <a href="./type/SendMessageAction.md">SendMessageAction</a>;

<a href="./constructor/contacts.found.md">contacts.found</a>#1aa1f784 results:Vector&lt;<a href="./type/Peer.md">Peer</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.Found.md">contacts.Found</a>;

<a href="./constructor/inputPrivacyKeyStatusTimestamp.md">inputPrivacyKeyStatusTimestamp</a>#4f96cb18 = <a href="./type/InputPrivacyKey.md">InputPrivacyKey</a>;
<a href="./constructor/inputPrivacyKeyChatInvite.md">inputPrivacyKeyChatInvite</a>#bdfb0426 = <a href="./type/InputPrivacyKey.md">InputPrivacyKey</a>;
<a href="./constructor/inputPrivacyKeyPhoneCall.md">inputPrivacyKeyPhoneCall</a>#fabadc5f = <a href="./type/InputPrivacyKey.md">InputPrivacyKey</a>;

<a href="./constructor/privacyKeyStatusTimestamp.md">privacyKeyStatusTimestamp</a>#bc2eab30 = <a href="./type/PrivacyKey.md">PrivacyKey</a>;
<a href="./constructor/privacyKeyChatInvite.md">privacyKeyChatInvite</a>#500e6dfa = <a href="./type/PrivacyKey.md">PrivacyKey</a>;
<a href="./constructor/privacyKeyPhoneCall.md">privacyKeyPhoneCall</a>#3d662b7b = <a href="./type/PrivacyKey.md">PrivacyKey</a>;

<a href="./constructor/inputPrivacyValueAllowContacts.md">inputPrivacyValueAllowContacts</a>#d09e07b = <a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>;
<a href="./constructor/inputPrivacyValueAllowAll.md">inputPrivacyValueAllowAll</a>#184b35ce = <a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>;
<a href="./constructor/inputPrivacyValueAllowUsers.md">inputPrivacyValueAllowUsers</a>#131cc67f users:Vector&lt;<a href="./type/InputUser.md">InputUser</a>&gt; = <a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>;
<a href="./constructor/inputPrivacyValueDisallowContacts.md">inputPrivacyValueDisallowContacts</a>#ba52007 = <a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>;
<a href="./constructor/inputPrivacyValueDisallowAll.md">inputPrivacyValueDisallowAll</a>#d66b66c9 = <a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>;
<a href="./constructor/inputPrivacyValueDisallowUsers.md">inputPrivacyValueDisallowUsers</a>#90110467 users:Vector&lt;<a href="./type/InputUser.md">InputUser</a>&gt; = <a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>;

<a href="./constructor/privacyValueAllowContacts.md">privacyValueAllowContacts</a>#fffe1bac = <a href="./type/PrivacyRule.md">PrivacyRule</a>;
<a href="./constructor/privacyValueAllowAll.md">privacyValueAllowAll</a>#65427b82 = <a href="./type/PrivacyRule.md">PrivacyRule</a>;
<a href="./constructor/privacyValueAllowUsers.md">privacyValueAllowUsers</a>#4d5bbe0c users:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/PrivacyRule.md">PrivacyRule</a>;
<a href="./constructor/privacyValueDisallowContacts.md">privacyValueDisallowContacts</a>#f888fa1a = <a href="./type/PrivacyRule.md">PrivacyRule</a>;
<a href="./constructor/privacyValueDisallowAll.md">privacyValueDisallowAll</a>#8b73e763 = <a href="./type/PrivacyRule.md">PrivacyRule</a>;
<a href="./constructor/privacyValueDisallowUsers.md">privacyValueDisallowUsers</a>#c7f49b7 users:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/PrivacyRule.md">PrivacyRule</a>;

<a href="./constructor/account.privacyRules.md">account.privacyRules</a>#554abb6f rules:Vector&lt;<a href="./type/PrivacyRule.md">PrivacyRule</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/account.PrivacyRules.md">account.PrivacyRules</a>;

<a href="./constructor/accountDaysTTL.md">accountDaysTTL</a>#b8d0afdf days:<a href="./type/int.md">int</a> = <a href="./type/AccountDaysTTL.md">AccountDaysTTL</a>;

<a href="./constructor/documentAttributeImageSize.md">documentAttributeImageSize</a>#6c37c15c w:<a href="./type/int.md">int</a> h:<a href="./type/int.md">int</a> = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;
<a href="./constructor/documentAttributeAnimated.md">documentAttributeAnimated</a>#11b58939 = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;
<a href="./constructor/documentAttributeSticker.md">documentAttributeSticker</a>#6319d612 flags:# mask:flags.1?<a href="./type/true.md">true</a> alt:<a href="./type/string.md">string</a> stickerset:<a href="./type/InputStickerSet.md">InputStickerSet</a> mask_coords:flags.0?<a href="./type/MaskCoords.md">MaskCoords</a> = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;
<a href="./constructor/documentAttributeVideo.md">documentAttributeVideo</a>#ef02ce6 flags:# round_message:flags.0?<a href="./type/true.md">true</a> duration:<a href="./type/int.md">int</a> w:<a href="./type/int.md">int</a> h:<a href="./type/int.md">int</a> = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;
<a href="./constructor/documentAttributeAudio.md">documentAttributeAudio</a>#9852f9c6 flags:# voice:flags.10?<a href="./type/true.md">true</a> duration:<a href="./type/int.md">int</a> title:flags.0?<a href="./type/string.md">string</a> performer:flags.1?<a href="./type/string.md">string</a> waveform:flags.2?<a href="./type/bytes.md">bytes</a> = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;
<a href="./constructor/documentAttributeFilename.md">documentAttributeFilename</a>#15590068 file_name:<a href="./type/string.md">string</a> = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;
<a href="./constructor/documentAttributeHasStickers.md">documentAttributeHasStickers</a>#9801d2f7 = <a href="./type/DocumentAttribute.md">DocumentAttribute</a>;

<a href="./constructor/messages.stickersNotModified.md">messages.stickersNotModified</a>#f1749a22 = <a href="./type/messages.Stickers.md">messages.Stickers</a>;
<a href="./constructor/messages.stickers.md">messages.stickers</a>#8a8ecd32 hash:<a href="./type/string.md">string</a> stickers:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/messages.Stickers.md">messages.Stickers</a>;

<a href="./constructor/stickerPack.md">stickerPack</a>#12b299d4 emoticon:<a href="./type/string.md">string</a> documents:Vector&lt;<a href="./type/long.md">long</a>&gt; = <a href="./type/StickerPack.md">StickerPack</a>;

<a href="./constructor/messages.allStickersNotModified.md">messages.allStickersNotModified</a>#e86602c3 = <a href="./type/messages.AllStickers.md">messages.AllStickers</a>;
<a href="./constructor/messages.allStickers.md">messages.allStickers</a>#edfd405f hash:<a href="./type/int.md">int</a> sets:Vector&lt;<a href="./type/StickerSet.md">StickerSet</a>&gt; = <a href="./type/messages.AllStickers.md">messages.AllStickers</a>;

<a href="./constructor/disabledFeature.md">disabledFeature</a>#ae636f24 feature:<a href="./type/string.md">string</a> description:<a href="./type/string.md">string</a> = <a href="./type/DisabledFeature.md">DisabledFeature</a>;

<a href="./constructor/messages.affectedMessages.md">messages.affectedMessages</a>#84d19185 pts:<a href="./type/int.md">int</a> pts_count:<a href="./type/int.md">int</a> = <a href="./type/messages.AffectedMessages.md">messages.AffectedMessages</a>;

<a href="./constructor/contactLinkUnknown.md">contactLinkUnknown</a>#5f4f9247 = <a href="./type/ContactLink.md">ContactLink</a>;
<a href="./constructor/contactLinkNone.md">contactLinkNone</a>#feedd3ad = <a href="./type/ContactLink.md">ContactLink</a>;
<a href="./constructor/contactLinkHasPhone.md">contactLinkHasPhone</a>#268f3f59 = <a href="./type/ContactLink.md">ContactLink</a>;
<a href="./constructor/contactLinkContact.md">contactLinkContact</a>#d502c2d0 = <a href="./type/ContactLink.md">ContactLink</a>;

<a href="./constructor/webPageEmpty.md">webPageEmpty</a>#eb1477e8 id:<a href="./type/long.md">long</a> = <a href="./type/WebPage.md">WebPage</a>;
<a href="./constructor/webPagePending.md">webPagePending</a>#c586da1c id:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> = <a href="./type/WebPage.md">WebPage</a>;
<a href="./constructor/webPage.md">webPage</a>#5f07b4bc flags:# id:<a href="./type/long.md">long</a> url:<a href="./type/string.md">string</a> display_url:<a href="./type/string.md">string</a> hash:<a href="./type/int.md">int</a> type:flags.0?<a href="./type/string.md">string</a> site_name:flags.1?<a href="./type/string.md">string</a> title:flags.2?<a href="./type/string.md">string</a> description:flags.3?<a href="./type/string.md">string</a> photo:flags.4?<a href="./type/Photo.md">Photo</a> embed_url:flags.5?<a href="./type/string.md">string</a> embed_type:flags.5?<a href="./type/string.md">string</a> embed_width:flags.6?<a href="./type/int.md">int</a> embed_height:flags.6?<a href="./type/int.md">int</a> duration:flags.7?<a href="./type/int.md">int</a> author:flags.8?<a href="./type/string.md">string</a> document:flags.9?<a href="./type/Document.md">Document</a> cached_page:flags.10?<a href="./type/Page.md">Page</a> = <a href="./type/WebPage.md">WebPage</a>;
<a href="./constructor/webPageNotModified.md">webPageNotModified</a>#85849473 = <a href="./type/WebPage.md">WebPage</a>;

<a href="./constructor/authorization.md">authorization</a>#7bf2e6f6 hash:<a href="./type/long.md">long</a> flags:<a href="./type/int.md">int</a> device_model:<a href="./type/string.md">string</a> platform:<a href="./type/string.md">string</a> system_version:<a href="./type/string.md">string</a> api_id:<a href="./type/int.md">int</a> app_name:<a href="./type/string.md">string</a> app_version:<a href="./type/string.md">string</a> date_created:<a href="./type/int.md">int</a> date_active:<a href="./type/int.md">int</a> ip:<a href="./type/string.md">string</a> country:<a href="./type/string.md">string</a> region:<a href="./type/string.md">string</a> = <a href="./type/Authorization.md">Authorization</a>;

<a href="./constructor/account.authorizations.md">account.authorizations</a>#1250abde authorizations:Vector&lt;<a href="./type/Authorization.md">Authorization</a>&gt; = <a href="./type/account.Authorizations.md">account.Authorizations</a>;

<a href="./constructor/account.noPassword.md">account.noPassword</a>#96dabc18 new_salt:<a href="./type/bytes.md">bytes</a> email_unconfirmed_pattern:<a href="./type/string.md">string</a> = <a href="./type/account.Password.md">account.Password</a>;
<a href="./constructor/account.password.md">account.password</a>#7c18141c current_salt:<a href="./type/bytes.md">bytes</a> new_salt:<a href="./type/bytes.md">bytes</a> hint:<a href="./type/string.md">string</a> has_recovery:<a href="./type/Bool.md">Bool</a> email_unconfirmed_pattern:<a href="./type/string.md">string</a> = <a href="./type/account.Password.md">account.Password</a>;

<a href="./constructor/account.passwordSettings.md">account.passwordSettings</a>#b7b72ab3 email:<a href="./type/string.md">string</a> = <a href="./type/account.PasswordSettings.md">account.PasswordSettings</a>;

<a href="./constructor/account.passwordInputSettings.md">account.passwordInputSettings</a>#86916deb flags:# new_salt:flags.0?<a href="./type/bytes.md">bytes</a> new_password_hash:flags.0?<a href="./type/bytes.md">bytes</a> hint:flags.0?<a href="./type/string.md">string</a> email:flags.1?<a href="./type/string.md">string</a> = <a href="./type/account.PasswordInputSettings.md">account.PasswordInputSettings</a>;

<a href="./constructor/auth.passwordRecovery.md">auth.passwordRecovery</a>#137948a5 email_pattern:<a href="./type/string.md">string</a> = <a href="./type/auth.PasswordRecovery.md">auth.PasswordRecovery</a>;

<a href="./constructor/receivedNotifyMessage.md">receivedNotifyMessage</a>#a384b779 id:<a href="./type/int.md">int</a> flags:<a href="./type/int.md">int</a> = <a href="./type/ReceivedNotifyMessage.md">ReceivedNotifyMessage</a>;

<a href="./constructor/chatInviteEmpty.md">chatInviteEmpty</a>#69df3769 = <a href="./type/ExportedChatInvite.md">ExportedChatInvite</a>;
<a href="./constructor/chatInviteExported.md">chatInviteExported</a>#fc2e05bc link:<a href="./type/string.md">string</a> = <a href="./type/ExportedChatInvite.md">ExportedChatInvite</a>;

<a href="./constructor/chatInviteAlready.md">chatInviteAlready</a>#5a686d7c chat:<a href="./type/Chat.md">Chat</a> = <a href="./type/ChatInvite.md">ChatInvite</a>;
<a href="./constructor/chatInvite.md">chatInvite</a>#db74f558 flags:# channel:flags.0?<a href="./type/true.md">true</a> broadcast:flags.1?<a href="./type/true.md">true</a> public:flags.2?<a href="./type/true.md">true</a> megagroup:flags.3?<a href="./type/true.md">true</a> title:<a href="./type/string.md">string</a> photo:<a href="./type/ChatPhoto.md">ChatPhoto</a> participants_count:<a href="./type/int.md">int</a> participants:flags.4?Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/ChatInvite.md">ChatInvite</a>;

<a href="./constructor/inputStickerSetEmpty.md">inputStickerSetEmpty</a>#ffb62b95 = <a href="./type/InputStickerSet.md">InputStickerSet</a>;
<a href="./constructor/inputStickerSetID.md">inputStickerSetID</a>#9de7a269 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputStickerSet.md">InputStickerSet</a>;
<a href="./constructor/inputStickerSetShortName.md">inputStickerSetShortName</a>#861cc8a0 short_name:<a href="./type/string.md">string</a> = <a href="./type/InputStickerSet.md">InputStickerSet</a>;

<a href="./constructor/stickerSet.md">stickerSet</a>#cd303b41 flags:# installed:flags.0?<a href="./type/true.md">true</a> archived:flags.1?<a href="./type/true.md">true</a> official:flags.2?<a href="./type/true.md">true</a> masks:flags.3?<a href="./type/true.md">true</a> id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> title:<a href="./type/string.md">string</a> short_name:<a href="./type/string.md">string</a> count:<a href="./type/int.md">int</a> hash:<a href="./type/int.md">int</a> = <a href="./type/StickerSet.md">StickerSet</a>;

<a href="./constructor/messages.stickerSet.md">messages.stickerSet</a>#b60a24a6 set:<a href="./type/StickerSet.md">StickerSet</a> packs:Vector&lt;<a href="./type/StickerPack.md">StickerPack</a>&gt; documents:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/messages.StickerSet.md">messages.StickerSet</a>;

<a href="./constructor/botCommand.md">botCommand</a>#c27ac8c7 command:<a href="./type/string.md">string</a> description:<a href="./type/string.md">string</a> = <a href="./type/BotCommand.md">BotCommand</a>;

<a href="./constructor/botInfo.md">botInfo</a>#98e81d3a user_id:<a href="./type/int.md">int</a> description:<a href="./type/string.md">string</a> commands:Vector&lt;<a href="./type/BotCommand.md">BotCommand</a>&gt; = <a href="./type/BotInfo.md">BotInfo</a>;

<a href="./constructor/keyboardButton.md">keyboardButton</a>#a2fa4880 text:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonUrl.md">keyboardButtonUrl</a>#258aff05 text:<a href="./type/string.md">string</a> url:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonCallback.md">keyboardButtonCallback</a>#683a5e46 text:<a href="./type/string.md">string</a> data:<a href="./type/bytes.md">bytes</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonRequestPhone.md">keyboardButtonRequestPhone</a>#b16a6c29 text:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonRequestGeoLocation.md">keyboardButtonRequestGeoLocation</a>#fc796b3f text:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonSwitchInline.md">keyboardButtonSwitchInline</a>#568a748 flags:# same_peer:flags.0?<a href="./type/true.md">true</a> text:<a href="./type/string.md">string</a> query:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonGame.md">keyboardButtonGame</a>#50f41ccf text:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;
<a href="./constructor/keyboardButtonBuy.md">keyboardButtonBuy</a>#afd93fbb text:<a href="./type/string.md">string</a> = <a href="./type/KeyboardButton.md">KeyboardButton</a>;

<a href="./constructor/keyboardButtonRow.md">keyboardButtonRow</a>#77608b83 buttons:Vector&lt;<a href="./type/KeyboardButton.md">KeyboardButton</a>&gt; = <a href="./type/KeyboardButtonRow.md">KeyboardButtonRow</a>;

<a href="./constructor/replyKeyboardHide.md">replyKeyboardHide</a>#a03e5b85 flags:# selective:flags.2?<a href="./type/true.md">true</a> = <a href="./type/ReplyMarkup.md">ReplyMarkup</a>;
<a href="./constructor/replyKeyboardForceReply.md">replyKeyboardForceReply</a>#f4108aa0 flags:# single_use:flags.1?<a href="./type/true.md">true</a> selective:flags.2?<a href="./type/true.md">true</a> = <a href="./type/ReplyMarkup.md">ReplyMarkup</a>;
<a href="./constructor/replyKeyboardMarkup.md">replyKeyboardMarkup</a>#3502758c flags:# resize:flags.0?<a href="./type/true.md">true</a> single_use:flags.1?<a href="./type/true.md">true</a> selective:flags.2?<a href="./type/true.md">true</a> rows:Vector&lt;<a href="./type/KeyboardButtonRow.md">KeyboardButtonRow</a>&gt; = <a href="./type/ReplyMarkup.md">ReplyMarkup</a>;
<a href="./constructor/replyInlineMarkup.md">replyInlineMarkup</a>#48a30254 rows:Vector&lt;<a href="./type/KeyboardButtonRow.md">KeyboardButtonRow</a>&gt; = <a href="./type/ReplyMarkup.md">ReplyMarkup</a>;

<a href="./constructor/messageEntityUnknown.md">messageEntityUnknown</a>#bb92ba95 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityMention.md">messageEntityMention</a>#fa04579d offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityHashtag.md">messageEntityHashtag</a>#6f635b0d offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityBotCommand.md">messageEntityBotCommand</a>#6cef8ac7 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityUrl.md">messageEntityUrl</a>#6ed02538 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityEmail.md">messageEntityEmail</a>#64e475c2 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityBold.md">messageEntityBold</a>#bd610bc9 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityItalic.md">messageEntityItalic</a>#826f8b60 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityCode.md">messageEntityCode</a>#28a20571 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityPre.md">messageEntityPre</a>#73924be0 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> language:<a href="./type/string.md">string</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityTextUrl.md">messageEntityTextUrl</a>#76a6d327 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> url:<a href="./type/string.md">string</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/messageEntityMentionName.md">messageEntityMentionName</a>#352dca58 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;
<a href="./constructor/inputMessageEntityMentionName.md">inputMessageEntityMentionName</a>#208e68c9 offset:<a href="./type/int.md">int</a> length:<a href="./type/int.md">int</a> user_id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/MessageEntity.md">MessageEntity</a>;

<a href="./constructor/inputChannelEmpty.md">inputChannelEmpty</a>#ee8c1e86 = <a href="./type/InputChannel.md">InputChannel</a>;
<a href="./constructor/inputChannel.md">inputChannel</a>#afeb712e channel_id:<a href="./type/int.md">int</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputChannel.md">InputChannel</a>;

<a href="./constructor/contacts.resolvedPeer.md">contacts.resolvedPeer</a>#7f077ad9 peer:<a href="./type/Peer.md">Peer</a> chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.ResolvedPeer.md">contacts.ResolvedPeer</a>;

<a href="./constructor/messageRange.md">messageRange</a>#ae30253 min_id:<a href="./type/int.md">int</a> max_id:<a href="./type/int.md">int</a> = <a href="./type/MessageRange.md">MessageRange</a>;

<a href="./constructor/updates.channelDifferenceEmpty.md">updates.channelDifferenceEmpty</a>#3e11affb flags:# final:flags.0?<a href="./type/true.md">true</a> pts:<a href="./type/int.md">int</a> timeout:flags.1?<a href="./type/int.md">int</a> = <a href="./type/updates.ChannelDifference.md">updates.ChannelDifference</a>;
<a href="./constructor/updates.channelDifferenceTooLong.md">updates.channelDifferenceTooLong</a>#410dee07 flags:# final:flags.0?<a href="./type/true.md">true</a> pts:<a href="./type/int.md">int</a> timeout:flags.1?<a href="./type/int.md">int</a> top_message:<a href="./type/int.md">int</a> read_inbox_max_id:<a href="./type/int.md">int</a> read_outbox_max_id:<a href="./type/int.md">int</a> unread_count:<a href="./type/int.md">int</a> messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/updates.ChannelDifference.md">updates.ChannelDifference</a>;
<a href="./constructor/updates.channelDifference.md">updates.channelDifference</a>#2064674e flags:# final:flags.0?<a href="./type/true.md">true</a> pts:<a href="./type/int.md">int</a> timeout:flags.1?<a href="./type/int.md">int</a> new_messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; other_updates:Vector&lt;<a href="./type/Update.md">Update</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/updates.ChannelDifference.md">updates.ChannelDifference</a>;

<a href="./constructor/channelMessagesFilterEmpty.md">channelMessagesFilterEmpty</a>#94d42ee7 = <a href="./type/ChannelMessagesFilter.md">ChannelMessagesFilter</a>;
<a href="./constructor/channelMessagesFilter.md">channelMessagesFilter</a>#cd77d957 flags:# exclude_new_messages:flags.1?<a href="./type/true.md">true</a> ranges:Vector&lt;<a href="./type/MessageRange.md">MessageRange</a>&gt; = <a href="./type/ChannelMessagesFilter.md">ChannelMessagesFilter</a>;

<a href="./constructor/channelParticipant.md">channelParticipant</a>#15ebac1d user_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChannelParticipant.md">ChannelParticipant</a>;
<a href="./constructor/channelParticipantSelf.md">channelParticipantSelf</a>#a3289a6d user_id:<a href="./type/int.md">int</a> inviter_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChannelParticipant.md">ChannelParticipant</a>;
<a href="./constructor/channelParticipantModerator.md">channelParticipantModerator</a>#91057fef user_id:<a href="./type/int.md">int</a> inviter_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChannelParticipant.md">ChannelParticipant</a>;
<a href="./constructor/channelParticipantEditor.md">channelParticipantEditor</a>#98192d61 user_id:<a href="./type/int.md">int</a> inviter_id:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChannelParticipant.md">ChannelParticipant</a>;
<a href="./constructor/channelParticipantKicked.md">channelParticipantKicked</a>#8cc5e69a user_id:<a href="./type/int.md">int</a> kicked_by:<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> = <a href="./type/ChannelParticipant.md">ChannelParticipant</a>;
<a href="./constructor/channelParticipantCreator.md">channelParticipantCreator</a>#e3e2e1f9 user_id:<a href="./type/int.md">int</a> = <a href="./type/ChannelParticipant.md">ChannelParticipant</a>;

<a href="./constructor/channelParticipantsRecent.md">channelParticipantsRecent</a>#de3f3c79 = <a href="./type/ChannelParticipantsFilter.md">ChannelParticipantsFilter</a>;
<a href="./constructor/channelParticipantsAdmins.md">channelParticipantsAdmins</a>#b4608969 = <a href="./type/ChannelParticipantsFilter.md">ChannelParticipantsFilter</a>;
<a href="./constructor/channelParticipantsKicked.md">channelParticipantsKicked</a>#3c37bb7a = <a href="./type/ChannelParticipantsFilter.md">ChannelParticipantsFilter</a>;
<a href="./constructor/channelParticipantsBots.md">channelParticipantsBots</a>#b0d1865b = <a href="./type/ChannelParticipantsFilter.md">ChannelParticipantsFilter</a>;

<a href="./constructor/channelRoleEmpty.md">channelRoleEmpty</a>#b285a0c6 = <a href="./type/ChannelParticipantRole.md">ChannelParticipantRole</a>;
<a href="./constructor/channelRoleModerator.md">channelRoleModerator</a>#9618d975 = <a href="./type/ChannelParticipantRole.md">ChannelParticipantRole</a>;
<a href="./constructor/channelRoleEditor.md">channelRoleEditor</a>#820bfe8c = <a href="./type/ChannelParticipantRole.md">ChannelParticipantRole</a>;

<a href="./constructor/channels.channelParticipants.md">channels.channelParticipants</a>#f56ee2a8 count:<a href="./type/int.md">int</a> participants:Vector&lt;<a href="./type/ChannelParticipant.md">ChannelParticipant</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/channels.ChannelParticipants.md">channels.ChannelParticipants</a>;

<a href="./constructor/channels.channelParticipant.md">channels.channelParticipant</a>#d0d9b163 participant:<a href="./type/ChannelParticipant.md">ChannelParticipant</a> users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/channels.ChannelParticipant.md">channels.ChannelParticipant</a>;

<a href="./constructor/help.termsOfService.md">help.termsOfService</a>#f1ee3e90 text:<a href="./type/string.md">string</a> = <a href="./type/help.TermsOfService.md">help.TermsOfService</a>;

<a href="./constructor/foundGif.md">foundGif</a>#162ecc1f url:<a href="./type/string.md">string</a> thumb_url:<a href="./type/string.md">string</a> content_url:<a href="./type/string.md">string</a> content_type:<a href="./type/string.md">string</a> w:<a href="./type/int.md">int</a> h:<a href="./type/int.md">int</a> = <a href="./type/FoundGif.md">FoundGif</a>;
<a href="./constructor/foundGifCached.md">foundGifCached</a>#9c750409 url:<a href="./type/string.md">string</a> photo:<a href="./type/Photo.md">Photo</a> document:<a href="./type/Document.md">Document</a> = <a href="./type/FoundGif.md">FoundGif</a>;

<a href="./constructor/messages.foundGifs.md">messages.foundGifs</a>#450a1c0a next_offset:<a href="./type/int.md">int</a> results:Vector&lt;<a href="./type/FoundGif.md">FoundGif</a>&gt; = <a href="./type/messages.FoundGifs.md">messages.FoundGifs</a>;

<a href="./constructor/messages.savedGifsNotModified.md">messages.savedGifsNotModified</a>#e8025ca2 = <a href="./type/messages.SavedGifs.md">messages.SavedGifs</a>;
<a href="./constructor/messages.savedGifs.md">messages.savedGifs</a>#2e0709a5 hash:<a href="./type/int.md">int</a> gifs:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/messages.SavedGifs.md">messages.SavedGifs</a>;

<a href="./constructor/inputBotInlineMessageMediaAuto.md">inputBotInlineMessageMediaAuto</a>#292fed13 flags:# caption:<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a>;
<a href="./constructor/inputBotInlineMessageText.md">inputBotInlineMessageText</a>#3dcd7a87 flags:# no_webpage:flags.0?<a href="./type/true.md">true</a> message:<a href="./type/string.md">string</a> entities:flags.1?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a>;
<a href="./constructor/inputBotInlineMessageMediaGeo.md">inputBotInlineMessageMediaGeo</a>#f4a59de1 flags:# geo_point:<a href="./type/InputGeoPoint.md">InputGeoPoint</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a>;
<a href="./constructor/inputBotInlineMessageMediaVenue.md">inputBotInlineMessageMediaVenue</a>#aaafadc8 flags:# geo_point:<a href="./type/InputGeoPoint.md">InputGeoPoint</a> title:<a href="./type/string.md">string</a> address:<a href="./type/string.md">string</a> provider:<a href="./type/string.md">string</a> venue_id:<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a>;
<a href="./constructor/inputBotInlineMessageMediaContact.md">inputBotInlineMessageMediaContact</a>#2daf01a7 flags:# phone_number:<a href="./type/string.md">string</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a>;
<a href="./constructor/inputBotInlineMessageGame.md">inputBotInlineMessageGame</a>#4b425864 flags:# reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a>;

<a href="./constructor/inputBotInlineResult.md">inputBotInlineResult</a>#2cbbe15a flags:# id:<a href="./type/string.md">string</a> type:<a href="./type/string.md">string</a> title:flags.1?<a href="./type/string.md">string</a> description:flags.2?<a href="./type/string.md">string</a> url:flags.3?<a href="./type/string.md">string</a> thumb_url:flags.4?<a href="./type/string.md">string</a> content_url:flags.5?<a href="./type/string.md">string</a> content_type:flags.5?<a href="./type/string.md">string</a> w:flags.6?<a href="./type/int.md">int</a> h:flags.6?<a href="./type/int.md">int</a> duration:flags.7?<a href="./type/int.md">int</a> send_message:<a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a> = <a href="./type/InputBotInlineResult.md">InputBotInlineResult</a>;
<a href="./constructor/inputBotInlineResultPhoto.md">inputBotInlineResultPhoto</a>#a8d864a7 id:<a href="./type/string.md">string</a> type:<a href="./type/string.md">string</a> photo:<a href="./type/InputPhoto.md">InputPhoto</a> send_message:<a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a> = <a href="./type/InputBotInlineResult.md">InputBotInlineResult</a>;
<a href="./constructor/inputBotInlineResultDocument.md">inputBotInlineResultDocument</a>#fff8fdc4 flags:# id:<a href="./type/string.md">string</a> type:<a href="./type/string.md">string</a> title:flags.1?<a href="./type/string.md">string</a> description:flags.2?<a href="./type/string.md">string</a> document:<a href="./type/InputDocument.md">InputDocument</a> send_message:<a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a> = <a href="./type/InputBotInlineResult.md">InputBotInlineResult</a>;
<a href="./constructor/inputBotInlineResultGame.md">inputBotInlineResultGame</a>#4fa417f2 id:<a href="./type/string.md">string</a> short_name:<a href="./type/string.md">string</a> send_message:<a href="./type/InputBotInlineMessage.md">InputBotInlineMessage</a> = <a href="./type/InputBotInlineResult.md">InputBotInlineResult</a>;

<a href="./constructor/botInlineMessageMediaAuto.md">botInlineMessageMediaAuto</a>#a74b15b flags:# caption:<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/BotInlineMessage.md">BotInlineMessage</a>;
<a href="./constructor/botInlineMessageText.md">botInlineMessageText</a>#8c7f65e2 flags:# no_webpage:flags.0?<a href="./type/true.md">true</a> message:<a href="./type/string.md">string</a> entities:flags.1?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/BotInlineMessage.md">BotInlineMessage</a>;
<a href="./constructor/botInlineMessageMediaGeo.md">botInlineMessageMediaGeo</a>#3a8fd8b8 flags:# geo:<a href="./type/GeoPoint.md">GeoPoint</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/BotInlineMessage.md">BotInlineMessage</a>;
<a href="./constructor/botInlineMessageMediaVenue.md">botInlineMessageMediaVenue</a>#4366232e flags:# geo:<a href="./type/GeoPoint.md">GeoPoint</a> title:<a href="./type/string.md">string</a> address:<a href="./type/string.md">string</a> provider:<a href="./type/string.md">string</a> venue_id:<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/BotInlineMessage.md">BotInlineMessage</a>;
<a href="./constructor/botInlineMessageMediaContact.md">botInlineMessageMediaContact</a>#35edb4d4 flags:# phone_number:<a href="./type/string.md">string</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/BotInlineMessage.md">BotInlineMessage</a>;

<a href="./constructor/botInlineResult.md">botInlineResult</a>#9bebaeb9 flags:# id:<a href="./type/string.md">string</a> type:<a href="./type/string.md">string</a> title:flags.1?<a href="./type/string.md">string</a> description:flags.2?<a href="./type/string.md">string</a> url:flags.3?<a href="./type/string.md">string</a> thumb_url:flags.4?<a href="./type/string.md">string</a> content_url:flags.5?<a href="./type/string.md">string</a> content_type:flags.5?<a href="./type/string.md">string</a> w:flags.6?<a href="./type/int.md">int</a> h:flags.6?<a href="./type/int.md">int</a> duration:flags.7?<a href="./type/int.md">int</a> send_message:<a href="./type/BotInlineMessage.md">BotInlineMessage</a> = <a href="./type/BotInlineResult.md">BotInlineResult</a>;
<a href="./constructor/botInlineMediaResult.md">botInlineMediaResult</a>#17db940b flags:# id:<a href="./type/string.md">string</a> type:<a href="./type/string.md">string</a> photo:flags.0?<a href="./type/Photo.md">Photo</a> document:flags.1?<a href="./type/Document.md">Document</a> title:flags.2?<a href="./type/string.md">string</a> description:flags.3?<a href="./type/string.md">string</a> send_message:<a href="./type/BotInlineMessage.md">BotInlineMessage</a> = <a href="./type/BotInlineResult.md">BotInlineResult</a>;

<a href="./constructor/messages.botResults.md">messages.botResults</a>#ccd3563d flags:# gallery:flags.0?<a href="./type/true.md">true</a> query_id:<a href="./type/long.md">long</a> next_offset:flags.1?<a href="./type/string.md">string</a> switch_pm:flags.2?<a href="./type/InlineBotSwitchPM.md">InlineBotSwitchPM</a> results:Vector&lt;<a href="./type/BotInlineResult.md">BotInlineResult</a>&gt; cache_time:<a href="./type/int.md">int</a> = <a href="./type/messages.BotResults.md">messages.BotResults</a>;

<a href="./constructor/exportedMessageLink.md">exportedMessageLink</a>#1f486803 link:<a href="./type/string.md">string</a> = <a href="./type/ExportedMessageLink.md">ExportedMessageLink</a>;

<a href="./constructor/messageFwdHeader.md">messageFwdHeader</a>#c786ddcb flags:# from_id:flags.0?<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> channel_id:flags.1?<a href="./type/int.md">int</a> channel_post:flags.2?<a href="./type/int.md">int</a> = <a href="./type/MessageFwdHeader.md">MessageFwdHeader</a>;

<a href="./constructor/auth.codeTypeSms.md">auth.codeTypeSms</a>#72a3158c = <a href="./type/auth.CodeType.md">auth.CodeType</a>;
<a href="./constructor/auth.codeTypeCall.md">auth.codeTypeCall</a>#741cd3e3 = <a href="./type/auth.CodeType.md">auth.CodeType</a>;
<a href="./constructor/auth.codeTypeFlashCall.md">auth.codeTypeFlashCall</a>#226ccefb = <a href="./type/auth.CodeType.md">auth.CodeType</a>;

<a href="./constructor/auth.sentCodeTypeApp.md">auth.sentCodeTypeApp</a>#3dbb5986 length:<a href="./type/int.md">int</a> = <a href="./type/auth.SentCodeType.md">auth.SentCodeType</a>;
<a href="./constructor/auth.sentCodeTypeSms.md">auth.sentCodeTypeSms</a>#c000bba2 length:<a href="./type/int.md">int</a> = <a href="./type/auth.SentCodeType.md">auth.SentCodeType</a>;
<a href="./constructor/auth.sentCodeTypeCall.md">auth.sentCodeTypeCall</a>#5353e5a7 length:<a href="./type/int.md">int</a> = <a href="./type/auth.SentCodeType.md">auth.SentCodeType</a>;
<a href="./constructor/auth.sentCodeTypeFlashCall.md">auth.sentCodeTypeFlashCall</a>#ab03c6d9 pattern:<a href="./type/string.md">string</a> = <a href="./type/auth.SentCodeType.md">auth.SentCodeType</a>;

<a href="./constructor/messages.botCallbackAnswer.md">messages.botCallbackAnswer</a>#36585ea4 flags:# alert:flags.1?<a href="./type/true.md">true</a> has_url:flags.3?<a href="./type/true.md">true</a> message:flags.0?<a href="./type/string.md">string</a> url:flags.2?<a href="./type/string.md">string</a> cache_time:<a href="./type/int.md">int</a> = <a href="./type/messages.BotCallbackAnswer.md">messages.BotCallbackAnswer</a>;

<a href="./constructor/messages.messageEditData.md">messages.messageEditData</a>#26b5dde6 flags:# caption:flags.0?<a href="./type/true.md">true</a> = <a href="./type/messages.MessageEditData.md">messages.MessageEditData</a>;

<a href="./constructor/inputBotInlineMessageID.md">inputBotInlineMessageID</a>#890c3d89 dc_id:<a href="./type/int.md">int</a> id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputBotInlineMessageID.md">InputBotInlineMessageID</a>;

<a href="./constructor/inlineBotSwitchPM.md">inlineBotSwitchPM</a>#3c20629f text:<a href="./type/string.md">string</a> start_param:<a href="./type/string.md">string</a> = <a href="./type/InlineBotSwitchPM.md">InlineBotSwitchPM</a>;

<a href="./constructor/messages.peerDialogs.md">messages.peerDialogs</a>#3371c354 dialogs:Vector&lt;<a href="./type/Dialog.md">Dialog</a>&gt; messages:Vector&lt;<a href="./type/Message.md">Message</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; state:<a href="./type/updates.State.md">updates.State</a> = <a href="./type/messages.PeerDialogs.md">messages.PeerDialogs</a>;

<a href="./constructor/topPeer.md">topPeer</a>#edcdc05b peer:<a href="./type/Peer.md">Peer</a> rating:<a href="./type/double.md">double</a> = <a href="./type/TopPeer.md">TopPeer</a>;

<a href="./constructor/topPeerCategoryBotsPM.md">topPeerCategoryBotsPM</a>#ab661b5b = <a href="./type/TopPeerCategory.md">TopPeerCategory</a>;
<a href="./constructor/topPeerCategoryBotsInline.md">topPeerCategoryBotsInline</a>#148677e2 = <a href="./type/TopPeerCategory.md">TopPeerCategory</a>;
<a href="./constructor/topPeerCategoryCorrespondents.md">topPeerCategoryCorrespondents</a>#637b7ed = <a href="./type/TopPeerCategory.md">TopPeerCategory</a>;
<a href="./constructor/topPeerCategoryGroups.md">topPeerCategoryGroups</a>#bd17a14a = <a href="./type/TopPeerCategory.md">TopPeerCategory</a>;
<a href="./constructor/topPeerCategoryChannels.md">topPeerCategoryChannels</a>#161d9628 = <a href="./type/TopPeerCategory.md">TopPeerCategory</a>;

<a href="./constructor/topPeerCategoryPeers.md">topPeerCategoryPeers</a>#fb834291 category:<a href="./type/TopPeerCategory.md">TopPeerCategory</a> count:<a href="./type/int.md">int</a> peers:Vector&lt;<a href="./type/TopPeer.md">TopPeer</a>&gt; = <a href="./type/TopPeerCategoryPeers.md">TopPeerCategoryPeers</a>;

<a href="./constructor/contacts.topPeersNotModified.md">contacts.topPeersNotModified</a>#de266ef5 = <a href="./type/contacts.TopPeers.md">contacts.TopPeers</a>;
<a href="./constructor/contacts.topPeers.md">contacts.topPeers</a>#70b772a8 categories:Vector&lt;<a href="./type/TopPeerCategoryPeers.md">TopPeerCategoryPeers</a>&gt; chats:Vector&lt;<a href="./type/Chat.md">Chat</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/contacts.TopPeers.md">contacts.TopPeers</a>;

<a href="./constructor/draftMessageEmpty.md">draftMessageEmpty</a>#ba4baec5 = <a href="./type/DraftMessage.md">DraftMessage</a>;
<a href="./constructor/draftMessage.md">draftMessage</a>#fd8e711f flags:# no_webpage:flags.1?<a href="./type/true.md">true</a> reply_to_msg_id:flags.0?<a href="./type/int.md">int</a> message:<a href="./type/string.md">string</a> entities:flags.3?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; date:<a href="./type/int.md">int</a> = <a href="./type/DraftMessage.md">DraftMessage</a>;

<a href="./constructor/messages.featuredStickersNotModified.md">messages.featuredStickersNotModified</a>#4ede3cf = <a href="./type/messages.FeaturedStickers.md">messages.FeaturedStickers</a>;
<a href="./constructor/messages.featuredStickers.md">messages.featuredStickers</a>#f89d88e5 hash:<a href="./type/int.md">int</a> sets:Vector&lt;<a href="./type/StickerSetCovered.md">StickerSetCovered</a>&gt; unread:Vector&lt;<a href="./type/long.md">long</a>&gt; = <a href="./type/messages.FeaturedStickers.md">messages.FeaturedStickers</a>;

<a href="./constructor/messages.recentStickersNotModified.md">messages.recentStickersNotModified</a>#b17f890 = <a href="./type/messages.RecentStickers.md">messages.RecentStickers</a>;
<a href="./constructor/messages.recentStickers.md">messages.recentStickers</a>#5ce20970 hash:<a href="./type/int.md">int</a> stickers:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/messages.RecentStickers.md">messages.RecentStickers</a>;

<a href="./constructor/messages.archivedStickers.md">messages.archivedStickers</a>#4fcba9c8 count:<a href="./type/int.md">int</a> sets:Vector&lt;<a href="./type/StickerSetCovered.md">StickerSetCovered</a>&gt; = <a href="./type/messages.ArchivedStickers.md">messages.ArchivedStickers</a>;

<a href="./constructor/messages.stickerSetInstallResultSuccess.md">messages.stickerSetInstallResultSuccess</a>#38641628 = <a href="./type/messages.StickerSetInstallResult.md">messages.StickerSetInstallResult</a>;
<a href="./constructor/messages.stickerSetInstallResultArchive.md">messages.stickerSetInstallResultArchive</a>#35e410a8 sets:Vector&lt;<a href="./type/StickerSetCovered.md">StickerSetCovered</a>&gt; = <a href="./type/messages.StickerSetInstallResult.md">messages.StickerSetInstallResult</a>;

<a href="./constructor/stickerSetCovered.md">stickerSetCovered</a>#6410a5d2 set:<a href="./type/StickerSet.md">StickerSet</a> cover:<a href="./type/Document.md">Document</a> = <a href="./type/StickerSetCovered.md">StickerSetCovered</a>;
<a href="./constructor/stickerSetMultiCovered.md">stickerSetMultiCovered</a>#3407e51b set:<a href="./type/StickerSet.md">StickerSet</a> covers:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/StickerSetCovered.md">StickerSetCovered</a>;

<a href="./constructor/maskCoords.md">maskCoords</a>#aed6dbb2 n:<a href="./type/int.md">int</a> x:<a href="./type/double.md">double</a> y:<a href="./type/double.md">double</a> zoom:<a href="./type/double.md">double</a> = <a href="./type/MaskCoords.md">MaskCoords</a>;

<a href="./constructor/inputStickeredMediaPhoto.md">inputStickeredMediaPhoto</a>#4a992157 id:<a href="./type/InputPhoto.md">InputPhoto</a> = <a href="./type/InputStickeredMedia.md">InputStickeredMedia</a>;
<a href="./constructor/inputStickeredMediaDocument.md">inputStickeredMediaDocument</a>#438865b id:<a href="./type/InputDocument.md">InputDocument</a> = <a href="./type/InputStickeredMedia.md">InputStickeredMedia</a>;

<a href="./constructor/game.md">game</a>#bdf9653b flags:# id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> short_name:<a href="./type/string.md">string</a> title:<a href="./type/string.md">string</a> description:<a href="./type/string.md">string</a> photo:<a href="./type/Photo.md">Photo</a> document:flags.0?<a href="./type/Document.md">Document</a> = <a href="./type/Game.md">Game</a>;

<a href="./constructor/inputGameID.md">inputGameID</a>#32c3e77 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputGame.md">InputGame</a>;
<a href="./constructor/inputGameShortName.md">inputGameShortName</a>#c331e80a bot_id:<a href="./type/InputUser.md">InputUser</a> short_name:<a href="./type/string.md">string</a> = <a href="./type/InputGame.md">InputGame</a>;

<a href="./constructor/highScore.md">highScore</a>#58fffcd0 pos:<a href="./type/int.md">int</a> user_id:<a href="./type/int.md">int</a> score:<a href="./type/int.md">int</a> = <a href="./type/HighScore.md">HighScore</a>;

<a href="./constructor/messages.highScores.md">messages.highScores</a>#9a3bfd99 scores:Vector&lt;<a href="./type/HighScore.md">HighScore</a>&gt; users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/messages.HighScores.md">messages.HighScores</a>;

<a href="./constructor/textEmpty.md">textEmpty</a>#dc3d824f = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textPlain.md">textPlain</a>#744694e0 text:<a href="./type/string.md">string</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textBold.md">textBold</a>#6724abc4 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textItalic.md">textItalic</a>#d912a59c text:<a href="./type/RichText.md">RichText</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textUnderline.md">textUnderline</a>#c12622c4 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textStrike.md">textStrike</a>#9bf8bb95 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textFixed.md">textFixed</a>#6c3f19b9 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textUrl.md">textUrl</a>#3c2884c1 text:<a href="./type/RichText.md">RichText</a> url:<a href="./type/string.md">string</a> webpage_id:<a href="./type/long.md">long</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textEmail.md">textEmail</a>#de5a0dd6 text:<a href="./type/RichText.md">RichText</a> email:<a href="./type/string.md">string</a> = <a href="./type/RichText.md">RichText</a>;
<a href="./constructor/textConcat.md">textConcat</a>#7e6260d7 texts:Vector&lt;<a href="./type/RichText.md">RichText</a>&gt; = <a href="./type/RichText.md">RichText</a>;

<a href="./constructor/pageBlockUnsupported.md">pageBlockUnsupported</a>#13567e8a = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockTitle.md">pageBlockTitle</a>#70abc3fd text:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockSubtitle.md">pageBlockSubtitle</a>#8ffa9a1f text:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockAuthorDate.md">pageBlockAuthorDate</a>#baafe5e0 author:<a href="./type/RichText.md">RichText</a> published_date:<a href="./type/int.md">int</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockHeader.md">pageBlockHeader</a>#bfd064ec text:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockSubheader.md">pageBlockSubheader</a>#f12bb6e1 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockParagraph.md">pageBlockParagraph</a>#467a0766 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockPreformatted.md">pageBlockPreformatted</a>#c070d93e text:<a href="./type/RichText.md">RichText</a> language:<a href="./type/string.md">string</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockFooter.md">pageBlockFooter</a>#48870999 text:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockDivider.md">pageBlockDivider</a>#db20b188 = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockAnchor.md">pageBlockAnchor</a>#ce0d37b0 name:<a href="./type/string.md">string</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockList.md">pageBlockList</a>#3a58c7f4 ordered:<a href="./type/Bool.md">Bool</a> items:Vector&lt;<a href="./type/RichText.md">RichText</a>&gt; = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockBlockquote.md">pageBlockBlockquote</a>#263d7c26 text:<a href="./type/RichText.md">RichText</a> caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockPullquote.md">pageBlockPullquote</a>#4f4456d3 text:<a href="./type/RichText.md">RichText</a> caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockPhoto.md">pageBlockPhoto</a>#e9c69982 photo_id:<a href="./type/long.md">long</a> caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockVideo.md">pageBlockVideo</a>#d9d71866 flags:# autoplay:flags.0?<a href="./type/true.md">true</a> loop:flags.1?<a href="./type/true.md">true</a> video_id:<a href="./type/long.md">long</a> caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockCover.md">pageBlockCover</a>#39f23300 cover:<a href="./type/PageBlock.md">PageBlock</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockEmbed.md">pageBlockEmbed</a>#cde200d1 flags:# full_width:flags.0?<a href="./type/true.md">true</a> allow_scrolling:flags.3?<a href="./type/true.md">true</a> url:flags.1?<a href="./type/string.md">string</a> html:flags.2?<a href="./type/string.md">string</a> poster_photo_id:flags.4?<a href="./type/long.md">long</a> w:<a href="./type/int.md">int</a> h:<a href="./type/int.md">int</a> caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockEmbedPost.md">pageBlockEmbedPost</a>#292c7be9 url:<a href="./type/string.md">string</a> webpage_id:<a href="./type/long.md">long</a> author_photo_id:<a href="./type/long.md">long</a> author:<a href="./type/string.md">string</a> date:<a href="./type/int.md">int</a> blocks:Vector&lt;<a href="./type/PageBlock.md">PageBlock</a>&gt; caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockCollage.md">pageBlockCollage</a>#8b31c4f items:Vector&lt;<a href="./type/PageBlock.md">PageBlock</a>&gt; caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockSlideshow.md">pageBlockSlideshow</a>#130c8963 items:Vector&lt;<a href="./type/PageBlock.md">PageBlock</a>&gt; caption:<a href="./type/RichText.md">RichText</a> = <a href="./type/PageBlock.md">PageBlock</a>;
<a href="./constructor/pageBlockChannel.md">pageBlockChannel</a>#ef1751b5 channel:<a href="./type/Chat.md">Chat</a> = <a href="./type/PageBlock.md">PageBlock</a>;

<a href="./constructor/pagePart.md">pagePart</a>#8dee6c44 blocks:Vector&lt;<a href="./type/PageBlock.md">PageBlock</a>&gt; photos:Vector&lt;<a href="./type/Photo.md">Photo</a>&gt; videos:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/Page.md">Page</a>;
<a href="./constructor/pageFull.md">pageFull</a>#d7a19d69 blocks:Vector&lt;<a href="./type/PageBlock.md">PageBlock</a>&gt; photos:Vector&lt;<a href="./type/Photo.md">Photo</a>&gt; videos:Vector&lt;<a href="./type/Document.md">Document</a>&gt; = <a href="./type/Page.md">Page</a>;

<a href="./constructor/phoneCallDiscardReasonMissed.md">phoneCallDiscardReasonMissed</a>#85e42301 = <a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a>;
<a href="./constructor/phoneCallDiscardReasonDisconnect.md">phoneCallDiscardReasonDisconnect</a>#e095c1a0 = <a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a>;
<a href="./constructor/phoneCallDiscardReasonHangup.md">phoneCallDiscardReasonHangup</a>#57adc690 = <a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a>;
<a href="./constructor/phoneCallDiscardReasonBusy.md">phoneCallDiscardReasonBusy</a>#faf7e8c9 = <a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a>;

<a href="./constructor/dataJSON.md">dataJSON</a>#7d748d04 data:<a href="./type/string.md">string</a> = <a href="./type/DataJSON.md">DataJSON</a>;

<a href="./constructor/labeledPrice.md">labeledPrice</a>#cb296bf8 label:<a href="./type/string.md">string</a> amount:<a href="./type/long.md">long</a> = <a href="./type/LabeledPrice.md">LabeledPrice</a>;

<a href="./constructor/invoice.md">invoice</a>#c30aa358 flags:# test:flags.0?<a href="./type/true.md">true</a> name_requested:flags.1?<a href="./type/true.md">true</a> phone_requested:flags.2?<a href="./type/true.md">true</a> email_requested:flags.3?<a href="./type/true.md">true</a> shipping_address_requested:flags.4?<a href="./type/true.md">true</a> flexible:flags.5?<a href="./type/true.md">true</a> currency:<a href="./type/string.md">string</a> prices:Vector&lt;<a href="./type/LabeledPrice.md">LabeledPrice</a>&gt; = <a href="./type/Invoice.md">Invoice</a>;

<a href="./constructor/paymentCharge.md">paymentCharge</a>#ea02c27e id:<a href="./type/string.md">string</a> provider_charge_id:<a href="./type/string.md">string</a> = <a href="./type/PaymentCharge.md">PaymentCharge</a>;

<a href="./constructor/postAddress.md">postAddress</a>#1e8caaeb street_line1:<a href="./type/string.md">string</a> street_line2:<a href="./type/string.md">string</a> city:<a href="./type/string.md">string</a> state:<a href="./type/string.md">string</a> country_iso2:<a href="./type/string.md">string</a> post_code:<a href="./type/string.md">string</a> = <a href="./type/PostAddress.md">PostAddress</a>;

<a href="./constructor/paymentRequestedInfo.md">paymentRequestedInfo</a>#909c3f94 flags:# name:flags.0?<a href="./type/string.md">string</a> phone:flags.1?<a href="./type/string.md">string</a> email:flags.2?<a href="./type/string.md">string</a> shipping_address:flags.3?<a href="./type/PostAddress.md">PostAddress</a> = <a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a>;

<a href="./constructor/paymentSavedCredentialsCard.md">paymentSavedCredentialsCard</a>#cdc27a1f id:<a href="./type/string.md">string</a> title:<a href="./type/string.md">string</a> = <a href="./type/PaymentSavedCredentials.md">PaymentSavedCredentials</a>;

<a href="./constructor/webDocument.md">webDocument</a>#c61acbd8 url:<a href="./type/string.md">string</a> access_hash:<a href="./type/long.md">long</a> size:<a href="./type/int.md">int</a> mime_type:<a href="./type/string.md">string</a> attributes:Vector&lt;<a href="./type/DocumentAttribute.md">DocumentAttribute</a>&gt; dc_id:<a href="./type/int.md">int</a> = <a href="./type/WebDocument.md">WebDocument</a>;

<a href="./constructor/inputWebDocument.md">inputWebDocument</a>#9bed434d url:<a href="./type/string.md">string</a> size:<a href="./type/int.md">int</a> mime_type:<a href="./type/string.md">string</a> attributes:Vector&lt;<a href="./type/DocumentAttribute.md">DocumentAttribute</a>&gt; = <a href="./type/InputWebDocument.md">InputWebDocument</a>;

<a href="./constructor/inputWebFileLocation.md">inputWebFileLocation</a>#c239d686 url:<a href="./type/string.md">string</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputWebFileLocation.md">InputWebFileLocation</a>;

<a href="./constructor/upload.webFile.md">upload.webFile</a>#21e753bc size:<a href="./type/int.md">int</a> mime_type:<a href="./type/string.md">string</a> file_type:<a href="./type/storage.FileType.md">storage.FileType</a> mtime:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/upload.WebFile.md">upload.WebFile</a>;

<a href="./constructor/payments.paymentForm.md">payments.paymentForm</a>#3f56aea3 flags:# can_save_credentials:flags.2?<a href="./type/true.md">true</a> password_missing:flags.3?<a href="./type/true.md">true</a> bot_id:<a href="./type/int.md">int</a> invoice:<a href="./type/Invoice.md">Invoice</a> provider_id:<a href="./type/int.md">int</a> url:<a href="./type/string.md">string</a> native_provider:flags.4?<a href="./type/string.md">string</a> native_params:flags.4?<a href="./type/DataJSON.md">DataJSON</a> saved_info:flags.0?<a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> saved_credentials:flags.1?<a href="./type/PaymentSavedCredentials.md">PaymentSavedCredentials</a> users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/payments.PaymentForm.md">payments.PaymentForm</a>;

<a href="./constructor/payments.validatedRequestedInfo.md">payments.validatedRequestedInfo</a>#d1451883 flags:# id:flags.0?<a href="./type/string.md">string</a> shipping_options:flags.1?Vector&lt;<a href="./type/ShippingOption.md">ShippingOption</a>&gt; = <a href="./type/payments.ValidatedRequestedInfo.md">payments.ValidatedRequestedInfo</a>;

<a href="./constructor/payments.paymentResult.md">payments.paymentResult</a>#4e5f810d updates:<a href="./type/Updates.md">Updates</a> = <a href="./type/payments.PaymentResult.md">payments.PaymentResult</a>;
<a href="./constructor/payments.paymentVerficationNeeded.md">payments.paymentVerficationNeeded</a>#6b56b921 url:<a href="./type/string.md">string</a> = <a href="./type/payments.PaymentResult.md">payments.PaymentResult</a>;

<a href="./constructor/payments.paymentReceipt.md">payments.paymentReceipt</a>#500911e1 flags:# date:<a href="./type/int.md">int</a> bot_id:<a href="./type/int.md">int</a> invoice:<a href="./type/Invoice.md">Invoice</a> provider_id:<a href="./type/int.md">int</a> info:flags.0?<a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> shipping:flags.1?<a href="./type/ShippingOption.md">ShippingOption</a> currency:<a href="./type/string.md">string</a> total_amount:<a href="./type/long.md">long</a> credentials_title:<a href="./type/string.md">string</a> users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/payments.PaymentReceipt.md">payments.PaymentReceipt</a>;

<a href="./constructor/payments.savedInfo.md">payments.savedInfo</a>#fb8fe43c flags:# has_saved_credentials:flags.1?<a href="./type/true.md">true</a> saved_info:flags.0?<a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> = <a href="./type/payments.SavedInfo.md">payments.SavedInfo</a>;

<a href="./constructor/inputPaymentCredentialsSaved.md">inputPaymentCredentialsSaved</a>#c10eb2cf id:<a href="./type/string.md">string</a> tmp_password:<a href="./type/bytes.md">bytes</a> = <a href="./type/InputPaymentCredentials.md">InputPaymentCredentials</a>;
<a href="./constructor/inputPaymentCredentials.md">inputPaymentCredentials</a>#3417d728 flags:# save:flags.0?<a href="./type/true.md">true</a> data:<a href="./type/DataJSON.md">DataJSON</a> = <a href="./type/InputPaymentCredentials.md">InputPaymentCredentials</a>;

<a href="./constructor/account.tmpPassword.md">account.tmpPassword</a>#db64fd34 tmp_password:<a href="./type/bytes.md">bytes</a> valid_until:<a href="./type/int.md">int</a> = <a href="./type/account.TmpPassword.md">account.TmpPassword</a>;

<a href="./constructor/shippingOption.md">shippingOption</a>#b6213cdf id:<a href="./type/string.md">string</a> title:<a href="./type/string.md">string</a> prices:Vector&lt;<a href="./type/LabeledPrice.md">LabeledPrice</a>&gt; = <a href="./type/ShippingOption.md">ShippingOption</a>;

<a href="./constructor/inputPhoneCall.md">inputPhoneCall</a>#1e36fded id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> = <a href="./type/InputPhoneCall.md">InputPhoneCall</a>;

<a href="./constructor/phoneCallEmpty.md">phoneCallEmpty</a>#5366c915 id:<a href="./type/long.md">long</a> = <a href="./type/PhoneCall.md">PhoneCall</a>;
<a href="./constructor/phoneCallWaiting.md">phoneCallWaiting</a>#1b8f4ad1 flags:# id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> receive_date:flags.0?<a href="./type/int.md">int</a> = <a href="./type/PhoneCall.md">PhoneCall</a>;
<a href="./constructor/phoneCallRequested.md">phoneCallRequested</a>#83761ce4 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> g_a_hash:<a href="./type/bytes.md">bytes</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> = <a href="./type/PhoneCall.md">PhoneCall</a>;
<a href="./constructor/phoneCallAccepted.md">phoneCallAccepted</a>#6d003d3f id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> g_b:<a href="./type/bytes.md">bytes</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> = <a href="./type/PhoneCall.md">PhoneCall</a>;
<a href="./constructor/phoneCall.md">phoneCall</a>#ffe6ab67 id:<a href="./type/long.md">long</a> access_hash:<a href="./type/long.md">long</a> date:<a href="./type/int.md">int</a> admin_id:<a href="./type/int.md">int</a> participant_id:<a href="./type/int.md">int</a> g_a_or_b:<a href="./type/bytes.md">bytes</a> key_fingerprint:<a href="./type/long.md">long</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> connection:<a href="./type/PhoneConnection.md">PhoneConnection</a> alternative_connections:Vector&lt;<a href="./type/PhoneConnection.md">PhoneConnection</a>&gt; start_date:<a href="./type/int.md">int</a> = <a href="./type/PhoneCall.md">PhoneCall</a>;
<a href="./constructor/phoneCallDiscarded.md">phoneCallDiscarded</a>#50ca4de1 flags:# need_rating:flags.2?<a href="./type/true.md">true</a> need_debug:flags.3?<a href="./type/true.md">true</a> id:<a href="./type/long.md">long</a> reason:flags.0?<a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a> duration:flags.1?<a href="./type/int.md">int</a> = <a href="./type/PhoneCall.md">PhoneCall</a>;

<a href="./constructor/phoneConnection.md">phoneConnection</a>#9d4c17c0 id:<a href="./type/long.md">long</a> ip:<a href="./type/string.md">string</a> ipv6:<a href="./type/string.md">string</a> port:<a href="./type/int.md">int</a> peer_tag:<a href="./type/bytes.md">bytes</a> = <a href="./type/PhoneConnection.md">PhoneConnection</a>;

<a href="./constructor/phoneCallProtocol.md">phoneCallProtocol</a>#a2bb35cb flags:# udp_p2p:flags.0?<a href="./type/true.md">true</a> udp_reflector:flags.1?<a href="./type/true.md">true</a> min_layer:<a href="./type/int.md">int</a> max_layer:<a href="./type/int.md">int</a> = <a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a>;

<a href="./constructor/phone.phoneCall.md">phone.phoneCall</a>#ec82e140 phone_call:<a href="./type/PhoneCall.md">PhoneCall</a> users:Vector&lt;<a href="./type/User.md">User</a>&gt; = <a href="./type/phone.PhoneCall.md">phone.PhoneCall</a>;

<a href="./constructor/upload.cdnFileReuploadNeeded.md">upload.cdnFileReuploadNeeded</a>#eea8e46e request_token:<a href="./type/bytes.md">bytes</a> = <a href="./type/upload.CdnFile.md">upload.CdnFile</a>;
<a href="./constructor/upload.cdnFile.md">upload.cdnFile</a>#a99fca4f bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/upload.CdnFile.md">upload.CdnFile</a>;

<a href="./constructor/cdnPublicKey.md">cdnPublicKey</a>#c982eaba dc_id:<a href="./type/int.md">int</a> public_key:<a href="./type/string.md">string</a> = <a href="./type/CdnPublicKey.md">CdnPublicKey</a>;

<a href="./constructor/cdnConfig.md">cdnConfig</a>#5725e40a public_keys:Vector&lt;<a href="./type/CdnPublicKey.md">CdnPublicKey</a>&gt; = <a href="./type/CdnConfig.md">CdnConfig</a>;

---functions---

<a href="./method/invokeAfterMsg.md">invokeAfterMsg</a>#cb9f372d msg_id:<a href="./type/long.md">long</a> query:!X = X;
<a href="./method/invokeAfterMsgs.md">invokeAfterMsgs</a>#3dc4b4f0 msg_ids:Vector&lt;<a href="./type/long.md">long</a>&gt; query:!X = X;
<a href="./method/initConnection.md">initConnection</a>#69796de9 api_id:<a href="./type/int.md">int</a> device_model:<a href="./type/string.md">string</a> system_version:<a href="./type/string.md">string</a> app_version:<a href="./type/string.md">string</a> lang_code:<a href="./type/string.md">string</a> query:!X = X;
<a href="./method/invokeWithLayer.md">invokeWithLayer</a>#da9b0d0d layer:<a href="./type/int.md">int</a> query:!X = X;
<a href="./method/invokeWithoutUpdates.md">invokeWithoutUpdates</a>#bf9459b7 query:!X = X;

<a href="./method/auth.checkPhone.md">auth.checkPhone</a>#6fe51dfb phone_number:<a href="./type/string.md">string</a> = <a href="./type/auth.CheckedPhone.md">auth.CheckedPhone</a>;
<a href="./method/auth.sendCode.md">auth.sendCode</a>#86aef0ec flags:# allow_flashcall:flags.0?<a href="./type/true.md">true</a> phone_number:<a href="./type/string.md">string</a> current_number:flags.0?<a href="./type/Bool.md">Bool</a> api_id:<a href="./type/int.md">int</a> api_hash:<a href="./type/string.md">string</a> = <a href="./type/auth.SentCode.md">auth.SentCode</a>;
<a href="./method/auth.signUp.md">auth.signUp</a>#1b067634 phone_number:<a href="./type/string.md">string</a> phone_code_hash:<a href="./type/string.md">string</a> phone_code:<a href="./type/string.md">string</a> first_name:<a href="./type/string.md">string</a> last_name:<a href="./type/string.md">string</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;
<a href="./method/auth.signIn.md">auth.signIn</a>#bcd51581 phone_number:<a href="./type/string.md">string</a> phone_code_hash:<a href="./type/string.md">string</a> phone_code:<a href="./type/string.md">string</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;
<a href="./method/auth.logOut.md">auth.logOut</a>#5717da40 = <a href="./type/Bool.md">Bool</a>;
<a href="./method/auth.resetAuthorizations.md">auth.resetAuthorizations</a>#9fab0d1a = <a href="./type/Bool.md">Bool</a>;
<a href="./method/auth.sendInvites.md">auth.sendInvites</a>#771c1d97 phone_numbers:Vector&lt;<a href="./type/string.md">string</a>&gt; message:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/auth.exportAuthorization.md">auth.exportAuthorization</a>#e5bfffcd dc_id:<a href="./type/int.md">int</a> = <a href="./type/auth.ExportedAuthorization.md">auth.ExportedAuthorization</a>;
<a href="./method/auth.importAuthorization.md">auth.importAuthorization</a>#e3ef9613 id:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;
<a href="./method/auth.bindTempAuthKey.md">auth.bindTempAuthKey</a>#cdd42a05 perm_auth_key_id:<a href="./type/long.md">long</a> nonce:<a href="./type/long.md">long</a> expires_at:<a href="./type/int.md">int</a> encrypted_message:<a href="./type/bytes.md">bytes</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/auth.importBotAuthorization.md">auth.importBotAuthorization</a>#67a3ff2c flags:<a href="./type/int.md">int</a> api_id:<a href="./type/int.md">int</a> api_hash:<a href="./type/string.md">string</a> bot_auth_token:<a href="./type/string.md">string</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;
<a href="./method/auth.checkPassword.md">auth.checkPassword</a>#a63011e password_hash:<a href="./type/bytes.md">bytes</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;
<a href="./method/auth.requestPasswordRecovery.md">auth.requestPasswordRecovery</a>#d897bc66 = <a href="./type/auth.PasswordRecovery.md">auth.PasswordRecovery</a>;
<a href="./method/auth.recoverPassword.md">auth.recoverPassword</a>#4ea56e92 code:<a href="./type/string.md">string</a> = <a href="./type/auth.Authorization.md">auth.Authorization</a>;
<a href="./method/auth.resendCode.md">auth.resendCode</a>#3ef1a9bf phone_number:<a href="./type/string.md">string</a> phone_code_hash:<a href="./type/string.md">string</a> = <a href="./type/auth.SentCode.md">auth.SentCode</a>;
<a href="./method/auth.cancelCode.md">auth.cancelCode</a>#1f040578 phone_number:<a href="./type/string.md">string</a> phone_code_hash:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/auth.dropTempAuthKeys.md">auth.dropTempAuthKeys</a>#8e48a188 except_auth_keys:Vector&lt;<a href="./type/long.md">long</a>&gt; = <a href="./type/Bool.md">Bool</a>;

<a href="./method/account.registerDevice.md">account.registerDevice</a>#637ea878 token_type:<a href="./type/int.md">int</a> token:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.unregisterDevice.md">account.unregisterDevice</a>#65c55b40 token_type:<a href="./type/int.md">int</a> token:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.updateNotifySettings.md">account.updateNotifySettings</a>#84be5b93 peer:<a href="./type/InputNotifyPeer.md">InputNotifyPeer</a> settings:<a href="./type/InputPeerNotifySettings.md">InputPeerNotifySettings</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.getNotifySettings.md">account.getNotifySettings</a>#12b3ad31 peer:<a href="./type/InputNotifyPeer.md">InputNotifyPeer</a> = <a href="./type/PeerNotifySettings.md">PeerNotifySettings</a>;
<a href="./method/account.resetNotifySettings.md">account.resetNotifySettings</a>#db7e1747 = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.updateProfile.md">account.updateProfile</a>#78515775 flags:# first_name:flags.0?<a href="./type/string.md">string</a> last_name:flags.1?<a href="./type/string.md">string</a> about:flags.2?<a href="./type/string.md">string</a> = <a href="./type/User.md">User</a>;
<a href="./method/account.updateStatus.md">account.updateStatus</a>#6628562c offline:<a href="./type/Bool.md">Bool</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.getWallPapers.md">account.getWallPapers</a>#c04cfac2 = Vector&lt;<a href="./type/WallPaper.md">WallPaper</a>&gt;;
<a href="./method/account.reportPeer.md">account.reportPeer</a>#ae189d5f peer:<a href="./type/InputPeer.md">InputPeer</a> reason:<a href="./type/ReportReason.md">ReportReason</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.checkUsername.md">account.checkUsername</a>#2714d86c username:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.updateUsername.md">account.updateUsername</a>#3e0bdd7c username:<a href="./type/string.md">string</a> = <a href="./type/User.md">User</a>;
<a href="./method/account.getPrivacy.md">account.getPrivacy</a>#dadbc950 key:<a href="./type/InputPrivacyKey.md">InputPrivacyKey</a> = <a href="./type/account.PrivacyRules.md">account.PrivacyRules</a>;
<a href="./method/account.setPrivacy.md">account.setPrivacy</a>#c9f81ce8 key:<a href="./type/InputPrivacyKey.md">InputPrivacyKey</a> rules:Vector&lt;<a href="./type/InputPrivacyRule.md">InputPrivacyRule</a>&gt; = <a href="./type/account.PrivacyRules.md">account.PrivacyRules</a>;
<a href="./method/account.deleteAccount.md">account.deleteAccount</a>#418d4e0b reason:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.getAccountTTL.md">account.getAccountTTL</a>#8fc711d = <a href="./type/AccountDaysTTL.md">AccountDaysTTL</a>;
<a href="./method/account.setAccountTTL.md">account.setAccountTTL</a>#2442485e ttl:<a href="./type/AccountDaysTTL.md">AccountDaysTTL</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.sendChangePhoneCode.md">account.sendChangePhoneCode</a>#8e57deb flags:# allow_flashcall:flags.0?<a href="./type/true.md">true</a> phone_number:<a href="./type/string.md">string</a> current_number:flags.0?<a href="./type/Bool.md">Bool</a> = <a href="./type/auth.SentCode.md">auth.SentCode</a>;
<a href="./method/account.changePhone.md">account.changePhone</a>#70c32edb phone_number:<a href="./type/string.md">string</a> phone_code_hash:<a href="./type/string.md">string</a> phone_code:<a href="./type/string.md">string</a> = <a href="./type/User.md">User</a>;
<a href="./method/account.updateDeviceLocked.md">account.updateDeviceLocked</a>#38df3532 period:<a href="./type/int.md">int</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.getAuthorizations.md">account.getAuthorizations</a>#e320c158 = <a href="./type/account.Authorizations.md">account.Authorizations</a>;
<a href="./method/account.resetAuthorization.md">account.resetAuthorization</a>#df77f3bc hash:<a href="./type/long.md">long</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.getPassword.md">account.getPassword</a>#548a30f5 = <a href="./type/account.Password.md">account.Password</a>;
<a href="./method/account.getPasswordSettings.md">account.getPasswordSettings</a>#bc8d11bb current_password_hash:<a href="./type/bytes.md">bytes</a> = <a href="./type/account.PasswordSettings.md">account.PasswordSettings</a>;
<a href="./method/account.updatePasswordSettings.md">account.updatePasswordSettings</a>#fa7c4b86 current_password_hash:<a href="./type/bytes.md">bytes</a> new_settings:<a href="./type/account.PasswordInputSettings.md">account.PasswordInputSettings</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.sendConfirmPhoneCode.md">account.sendConfirmPhoneCode</a>#1516d7bd flags:# allow_flashcall:flags.0?<a href="./type/true.md">true</a> hash:<a href="./type/string.md">string</a> current_number:flags.0?<a href="./type/Bool.md">Bool</a> = <a href="./type/auth.SentCode.md">auth.SentCode</a>;
<a href="./method/account.confirmPhone.md">account.confirmPhone</a>#5f2178c3 phone_code_hash:<a href="./type/string.md">string</a> phone_code:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/account.getTmpPassword.md">account.getTmpPassword</a>#4a82327e password_hash:<a href="./type/bytes.md">bytes</a> period:<a href="./type/int.md">int</a> = <a href="./type/account.TmpPassword.md">account.TmpPassword</a>;

<a href="./method/users.getUsers.md">users.getUsers</a>#d91a548 id:Vector&lt;<a href="./type/InputUser.md">InputUser</a>&gt; = Vector&lt;<a href="./type/User.md">User</a>&gt;;
<a href="./method/users.getFullUser.md">users.getFullUser</a>#ca30a5b1 id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/UserFull.md">UserFull</a>;

<a href="./method/contacts.getStatuses.md">contacts.getStatuses</a>#c4a353ee = Vector&lt;<a href="./type/ContactStatus.md">ContactStatus</a>&gt;;
<a href="./method/contacts.getContacts.md">contacts.getContacts</a>#22c6aa08 hash:<a href="./type/string.md">string</a> = <a href="./type/contacts.Contacts.md">contacts.Contacts</a>;
<a href="./method/contacts.importContacts.md">contacts.importContacts</a>#da30b32d contacts:Vector&lt;<a href="./type/InputContact.md">InputContact</a>&gt; replace:<a href="./type/Bool.md">Bool</a> = <a href="./type/contacts.ImportedContacts.md">contacts.ImportedContacts</a>;
<a href="./method/contacts.deleteContact.md">contacts.deleteContact</a>#8e953744 id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/contacts.Link.md">contacts.Link</a>;
<a href="./method/contacts.deleteContacts.md">contacts.deleteContacts</a>#59ab389e id:Vector&lt;<a href="./type/InputUser.md">InputUser</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/contacts.block.md">contacts.block</a>#332b49fc id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/contacts.unblock.md">contacts.unblock</a>#e54100bd id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/contacts.getBlocked.md">contacts.getBlocked</a>#f57c350f offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/contacts.Blocked.md">contacts.Blocked</a>;
<a href="./method/contacts.exportCard.md">contacts.exportCard</a>#84e53737 = Vector&lt;<a href="./type/int.md">int</a>&gt;;
<a href="./method/contacts.importCard.md">contacts.importCard</a>#4fe196fe export_card:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/User.md">User</a>;
<a href="./method/contacts.search.md">contacts.search</a>#11f812d8 q:<a href="./type/string.md">string</a> limit:<a href="./type/int.md">int</a> = <a href="./type/contacts.Found.md">contacts.Found</a>;
<a href="./method/contacts.resolveUsername.md">contacts.resolveUsername</a>#f93ccba3 username:<a href="./type/string.md">string</a> = <a href="./type/contacts.ResolvedPeer.md">contacts.ResolvedPeer</a>;
<a href="./method/contacts.getTopPeers.md">contacts.getTopPeers</a>#d4982db5 flags:# correspondents:flags.0?<a href="./type/true.md">true</a> bots_pm:flags.1?<a href="./type/true.md">true</a> bots_inline:flags.2?<a href="./type/true.md">true</a> groups:flags.10?<a href="./type/true.md">true</a> channels:flags.15?<a href="./type/true.md">true</a> offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> hash:<a href="./type/int.md">int</a> = <a href="./type/contacts.TopPeers.md">contacts.TopPeers</a>;
<a href="./method/contacts.resetTopPeerRating.md">contacts.resetTopPeerRating</a>#1ae373ac category:<a href="./type/TopPeerCategory.md">TopPeerCategory</a> peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/Bool.md">Bool</a>;

<a href="./method/messages.getMessages.md">messages.getMessages</a>#4222fa74 id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./method/messages.getDialogs.md">messages.getDialogs</a>#191ba9c5 flags:# exclude_pinned:flags.0?<a href="./type/true.md">true</a> offset_date:<a href="./type/int.md">int</a> offset_id:<a href="./type/int.md">int</a> offset_peer:<a href="./type/InputPeer.md">InputPeer</a> limit:<a href="./type/int.md">int</a> = <a href="./type/messages.Dialogs.md">messages.Dialogs</a>;
<a href="./method/messages.getHistory.md">messages.getHistory</a>#afa92846 peer:<a href="./type/InputPeer.md">InputPeer</a> offset_id:<a href="./type/int.md">int</a> offset_date:<a href="./type/int.md">int</a> add_offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> max_id:<a href="./type/int.md">int</a> min_id:<a href="./type/int.md">int</a> = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./method/messages.search.md">messages.search</a>#d4569248 flags:# peer:<a href="./type/InputPeer.md">InputPeer</a> q:<a href="./type/string.md">string</a> filter:<a href="./type/MessagesFilter.md">MessagesFilter</a> min_date:<a href="./type/int.md">int</a> max_date:<a href="./type/int.md">int</a> offset:<a href="./type/int.md">int</a> max_id:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./method/messages.readHistory.md">messages.readHistory</a>#e306d3a peer:<a href="./type/InputPeer.md">InputPeer</a> max_id:<a href="./type/int.md">int</a> = <a href="./type/messages.AffectedMessages.md">messages.AffectedMessages</a>;
<a href="./method/messages.deleteHistory.md">messages.deleteHistory</a>#1c015b09 flags:# just_clear:flags.0?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> max_id:<a href="./type/int.md">int</a> = <a href="./type/messages.AffectedHistory.md">messages.AffectedHistory</a>;
<a href="./method/messages.deleteMessages.md">messages.deleteMessages</a>#e58e95d2 flags:# revoke:flags.0?<a href="./type/true.md">true</a> id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.AffectedMessages.md">messages.AffectedMessages</a>;
<a href="./method/messages.receivedMessages.md">messages.receivedMessages</a>#5a954c0 max_id:<a href="./type/int.md">int</a> = Vector&lt;<a href="./type/ReceivedNotifyMessage.md">ReceivedNotifyMessage</a>&gt;;
<a href="./method/messages.setTyping.md">messages.setTyping</a>#a3825e50 peer:<a href="./type/InputPeer.md">InputPeer</a> action:<a href="./type/SendMessageAction.md">SendMessageAction</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.sendMessage.md">messages.sendMessage</a>#fa88427a flags:# no_webpage:flags.1?<a href="./type/true.md">true</a> silent:flags.5?<a href="./type/true.md">true</a> background:flags.6?<a href="./type/true.md">true</a> clear_draft:flags.7?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> reply_to_msg_id:flags.0?<a href="./type/int.md">int</a> message:<a href="./type/string.md">string</a> random_id:<a href="./type/long.md">long</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.3?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.sendMedia.md">messages.sendMedia</a>#c8f16791 flags:# silent:flags.5?<a href="./type/true.md">true</a> background:flags.6?<a href="./type/true.md">true</a> clear_draft:flags.7?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> reply_to_msg_id:flags.0?<a href="./type/int.md">int</a> media:<a href="./type/InputMedia.md">InputMedia</a> random_id:<a href="./type/long.md">long</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.forwardMessages.md">messages.forwardMessages</a>#708e0195 flags:# silent:flags.5?<a href="./type/true.md">true</a> background:flags.6?<a href="./type/true.md">true</a> with_my_score:flags.8?<a href="./type/true.md">true</a> from_peer:<a href="./type/InputPeer.md">InputPeer</a> id:Vector&lt;<a href="./type/int.md">int</a>&gt; random_id:Vector&lt;<a href="./type/long.md">long</a>&gt; to_peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.reportSpam.md">messages.reportSpam</a>#cf1592db peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.hideReportSpam.md">messages.hideReportSpam</a>#a8f1709b peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getPeerSettings.md">messages.getPeerSettings</a>#3672e09c peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/PeerSettings.md">PeerSettings</a>;
<a href="./method/messages.getChats.md">messages.getChats</a>#3c6aa187 id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.Chats.md">messages.Chats</a>;
<a href="./method/messages.getFullChat.md">messages.getFullChat</a>#3b831c66 chat_id:<a href="./type/int.md">int</a> = <a href="./type/messages.ChatFull.md">messages.ChatFull</a>;
<a href="./method/messages.editChatTitle.md">messages.editChatTitle</a>#dc452855 chat_id:<a href="./type/int.md">int</a> title:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.editChatPhoto.md">messages.editChatPhoto</a>#ca4c79d8 chat_id:<a href="./type/int.md">int</a> photo:<a href="./type/InputChatPhoto.md">InputChatPhoto</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.addChatUser.md">messages.addChatUser</a>#f9a0aa09 chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/InputUser.md">InputUser</a> fwd_limit:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.deleteChatUser.md">messages.deleteChatUser</a>#e0611f16 chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.createChat.md">messages.createChat</a>#9cb126e users:Vector&lt;<a href="./type/InputUser.md">InputUser</a>&gt; title:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.forwardMessage.md">messages.forwardMessage</a>#33963bf9 peer:<a href="./type/InputPeer.md">InputPeer</a> id:<a href="./type/int.md">int</a> random_id:<a href="./type/long.md">long</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.getDhConfig.md">messages.getDhConfig</a>#26cf8950 version:<a href="./type/int.md">int</a> random_length:<a href="./type/int.md">int</a> = <a href="./type/messages.DhConfig.md">messages.DhConfig</a>;
<a href="./method/messages.requestEncryption.md">messages.requestEncryption</a>#f64daf43 user_id:<a href="./type/InputUser.md">InputUser</a> random_id:<a href="./type/int.md">int</a> g_a:<a href="./type/bytes.md">bytes</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;
<a href="./method/messages.acceptEncryption.md">messages.acceptEncryption</a>#3dbc0415 peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> g_b:<a href="./type/bytes.md">bytes</a> key_fingerprint:<a href="./type/long.md">long</a> = <a href="./type/EncryptedChat.md">EncryptedChat</a>;
<a href="./method/messages.discardEncryption.md">messages.discardEncryption</a>#edd923c5 chat_id:<a href="./type/int.md">int</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.setEncryptedTyping.md">messages.setEncryptedTyping</a>#791451ed peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> typing:<a href="./type/Bool.md">Bool</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.readEncryptedHistory.md">messages.readEncryptedHistory</a>#7f4b690a peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> max_date:<a href="./type/int.md">int</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.sendEncrypted.md">messages.sendEncrypted</a>#a9776773 peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> random_id:<a href="./type/long.md">long</a> data:<a href="./type/bytes.md">bytes</a> = <a href="./type/messages.SentEncryptedMessage.md">messages.SentEncryptedMessage</a>;
<a href="./method/messages.sendEncryptedFile.md">messages.sendEncryptedFile</a>#9a901b66 peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> random_id:<a href="./type/long.md">long</a> data:<a href="./type/bytes.md">bytes</a> file:<a href="./type/InputEncryptedFile.md">InputEncryptedFile</a> = <a href="./type/messages.SentEncryptedMessage.md">messages.SentEncryptedMessage</a>;
<a href="./method/messages.sendEncryptedService.md">messages.sendEncryptedService</a>#32d439a4 peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> random_id:<a href="./type/long.md">long</a> data:<a href="./type/bytes.md">bytes</a> = <a href="./type/messages.SentEncryptedMessage.md">messages.SentEncryptedMessage</a>;
<a href="./method/messages.receivedQueue.md">messages.receivedQueue</a>#55a5bb66 max_qts:<a href="./type/int.md">int</a> = Vector&lt;<a href="./type/long.md">long</a>&gt;;
<a href="./method/messages.reportEncryptedSpam.md">messages.reportEncryptedSpam</a>#4b0c8c0f peer:<a href="./type/InputEncryptedChat.md">InputEncryptedChat</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.readMessageContents.md">messages.readMessageContents</a>#36a73f77 id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.AffectedMessages.md">messages.AffectedMessages</a>;
<a href="./method/messages.getAllStickers.md">messages.getAllStickers</a>#1c9618b1 hash:<a href="./type/int.md">int</a> = <a href="./type/messages.AllStickers.md">messages.AllStickers</a>;
<a href="./method/messages.getWebPagePreview.md">messages.getWebPagePreview</a>#25223e24 message:<a href="./type/string.md">string</a> = <a href="./type/MessageMedia.md">MessageMedia</a>;
<a href="./method/messages.exportChatInvite.md">messages.exportChatInvite</a>#7d885289 chat_id:<a href="./type/int.md">int</a> = <a href="./type/ExportedChatInvite.md">ExportedChatInvite</a>;
<a href="./method/messages.checkChatInvite.md">messages.checkChatInvite</a>#3eadb1bb hash:<a href="./type/string.md">string</a> = <a href="./type/ChatInvite.md">ChatInvite</a>;
<a href="./method/messages.importChatInvite.md">messages.importChatInvite</a>#6c50051c hash:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.getStickerSet.md">messages.getStickerSet</a>#2619a90e stickerset:<a href="./type/InputStickerSet.md">InputStickerSet</a> = <a href="./type/messages.StickerSet.md">messages.StickerSet</a>;
<a href="./method/messages.installStickerSet.md">messages.installStickerSet</a>#c78fe460 stickerset:<a href="./type/InputStickerSet.md">InputStickerSet</a> archived:<a href="./type/Bool.md">Bool</a> = <a href="./type/messages.StickerSetInstallResult.md">messages.StickerSetInstallResult</a>;
<a href="./method/messages.uninstallStickerSet.md">messages.uninstallStickerSet</a>#f96e55de stickerset:<a href="./type/InputStickerSet.md">InputStickerSet</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.startBot.md">messages.startBot</a>#e6df7378 bot:<a href="./type/InputUser.md">InputUser</a> peer:<a href="./type/InputPeer.md">InputPeer</a> random_id:<a href="./type/long.md">long</a> start_param:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.getMessagesViews.md">messages.getMessagesViews</a>#c4c8a55d peer:<a href="./type/InputPeer.md">InputPeer</a> id:Vector&lt;<a href="./type/int.md">int</a>&gt; increment:<a href="./type/Bool.md">Bool</a> = Vector&lt;<a href="./type/int.md">int</a>&gt;;
<a href="./method/messages.toggleChatAdmins.md">messages.toggleChatAdmins</a>#ec8bd9e1 chat_id:<a href="./type/int.md">int</a> enabled:<a href="./type/Bool.md">Bool</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.editChatAdmin.md">messages.editChatAdmin</a>#a9e69f2e chat_id:<a href="./type/int.md">int</a> user_id:<a href="./type/InputUser.md">InputUser</a> is_admin:<a href="./type/Bool.md">Bool</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.migrateChat.md">messages.migrateChat</a>#15a3b8e3 chat_id:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.searchGlobal.md">messages.searchGlobal</a>#9e3cacb0 q:<a href="./type/string.md">string</a> offset_date:<a href="./type/int.md">int</a> offset_peer:<a href="./type/InputPeer.md">InputPeer</a> offset_id:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./method/messages.reorderStickerSets.md">messages.reorderStickerSets</a>#78337739 flags:# masks:flags.0?<a href="./type/true.md">true</a> order:Vector&lt;<a href="./type/long.md">long</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getDocumentByHash.md">messages.getDocumentByHash</a>#338e2464 sha256:<a href="./type/bytes.md">bytes</a> size:<a href="./type/int.md">int</a> mime_type:<a href="./type/string.md">string</a> = <a href="./type/Document.md">Document</a>;
<a href="./method/messages.searchGifs.md">messages.searchGifs</a>#bf9a776b q:<a href="./type/string.md">string</a> offset:<a href="./type/int.md">int</a> = <a href="./type/messages.FoundGifs.md">messages.FoundGifs</a>;
<a href="./method/messages.getSavedGifs.md">messages.getSavedGifs</a>#83bf3d52 hash:<a href="./type/int.md">int</a> = <a href="./type/messages.SavedGifs.md">messages.SavedGifs</a>;
<a href="./method/messages.saveGif.md">messages.saveGif</a>#327a30cb id:<a href="./type/InputDocument.md">InputDocument</a> unsave:<a href="./type/Bool.md">Bool</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getInlineBotResults.md">messages.getInlineBotResults</a>#514e999d flags:# bot:<a href="./type/InputUser.md">InputUser</a> peer:<a href="./type/InputPeer.md">InputPeer</a> geo_point:flags.0?<a href="./type/InputGeoPoint.md">InputGeoPoint</a> query:<a href="./type/string.md">string</a> offset:<a href="./type/string.md">string</a> = <a href="./type/messages.BotResults.md">messages.BotResults</a>;
<a href="./method/messages.setInlineBotResults.md">messages.setInlineBotResults</a>#eb5ea206 flags:# gallery:flags.0?<a href="./type/true.md">true</a> private:flags.1?<a href="./type/true.md">true</a> query_id:<a href="./type/long.md">long</a> results:Vector&lt;<a href="./type/InputBotInlineResult.md">InputBotInlineResult</a>&gt; cache_time:<a href="./type/int.md">int</a> next_offset:flags.2?<a href="./type/string.md">string</a> switch_pm:flags.3?<a href="./type/InlineBotSwitchPM.md">InlineBotSwitchPM</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.sendInlineBotResult.md">messages.sendInlineBotResult</a>#b16e06fe flags:# silent:flags.5?<a href="./type/true.md">true</a> background:flags.6?<a href="./type/true.md">true</a> clear_draft:flags.7?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> reply_to_msg_id:flags.0?<a href="./type/int.md">int</a> random_id:<a href="./type/long.md">long</a> query_id:<a href="./type/long.md">long</a> id:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.getMessageEditData.md">messages.getMessageEditData</a>#fda68d36 peer:<a href="./type/InputPeer.md">InputPeer</a> id:<a href="./type/int.md">int</a> = <a href="./type/messages.MessageEditData.md">messages.MessageEditData</a>;
<a href="./method/messages.editMessage.md">messages.editMessage</a>#ce91e4ca flags:# no_webpage:flags.1?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> id:<a href="./type/int.md">int</a> message:flags.11?<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.3?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.editInlineBotMessage.md">messages.editInlineBotMessage</a>#130c2c85 flags:# no_webpage:flags.1?<a href="./type/true.md">true</a> id:<a href="./type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> message:flags.11?<a href="./type/string.md">string</a> reply_markup:flags.2?<a href="./type/ReplyMarkup.md">ReplyMarkup</a> entities:flags.3?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getBotCallbackAnswer.md">messages.getBotCallbackAnswer</a>#810a9fec flags:# game:flags.1?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> msg_id:<a href="./type/int.md">int</a> data:flags.0?<a href="./type/bytes.md">bytes</a> = <a href="./type/messages.BotCallbackAnswer.md">messages.BotCallbackAnswer</a>;
<a href="./method/messages.setBotCallbackAnswer.md">messages.setBotCallbackAnswer</a>#d58f130a flags:# alert:flags.1?<a href="./type/true.md">true</a> query_id:<a href="./type/long.md">long</a> message:flags.0?<a href="./type/string.md">string</a> url:flags.2?<a href="./type/string.md">string</a> cache_time:<a href="./type/int.md">int</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getPeerDialogs.md">messages.getPeerDialogs</a>#2d9776b9 peers:Vector&lt;<a href="./type/InputPeer.md">InputPeer</a>&gt; = <a href="./type/messages.PeerDialogs.md">messages.PeerDialogs</a>;
<a href="./method/messages.saveDraft.md">messages.saveDraft</a>#bc39e14b flags:# no_webpage:flags.1?<a href="./type/true.md">true</a> reply_to_msg_id:flags.0?<a href="./type/int.md">int</a> peer:<a href="./type/InputPeer.md">InputPeer</a> message:<a href="./type/string.md">string</a> entities:flags.3?Vector&lt;<a href="./type/MessageEntity.md">MessageEntity</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getAllDrafts.md">messages.getAllDrafts</a>#6a3f8d65 = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.getFeaturedStickers.md">messages.getFeaturedStickers</a>#2dacca4f hash:<a href="./type/int.md">int</a> = <a href="./type/messages.FeaturedStickers.md">messages.FeaturedStickers</a>;
<a href="./method/messages.readFeaturedStickers.md">messages.readFeaturedStickers</a>#5b118126 id:Vector&lt;<a href="./type/long.md">long</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getRecentStickers.md">messages.getRecentStickers</a>#5ea192c9 flags:# attached:flags.0?<a href="./type/true.md">true</a> hash:<a href="./type/int.md">int</a> = <a href="./type/messages.RecentStickers.md">messages.RecentStickers</a>;
<a href="./method/messages.saveRecentSticker.md">messages.saveRecentSticker</a>#392718f8 flags:# attached:flags.0?<a href="./type/true.md">true</a> id:<a href="./type/InputDocument.md">InputDocument</a> unsave:<a href="./type/Bool.md">Bool</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.clearRecentStickers.md">messages.clearRecentStickers</a>#8999602d flags:# attached:flags.0?<a href="./type/true.md">true</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getArchivedStickers.md">messages.getArchivedStickers</a>#57f17692 flags:# masks:flags.0?<a href="./type/true.md">true</a> offset_id:<a href="./type/long.md">long</a> limit:<a href="./type/int.md">int</a> = <a href="./type/messages.ArchivedStickers.md">messages.ArchivedStickers</a>;
<a href="./method/messages.getMaskStickers.md">messages.getMaskStickers</a>#65b8c79f hash:<a href="./type/int.md">int</a> = <a href="./type/messages.AllStickers.md">messages.AllStickers</a>;
<a href="./method/messages.getAttachedStickers.md">messages.getAttachedStickers</a>#cc5b67cc media:<a href="./type/InputStickeredMedia.md">InputStickeredMedia</a> = Vector&lt;<a href="./type/StickerSetCovered.md">StickerSetCovered</a>&gt;;
<a href="./method/messages.setGameScore.md">messages.setGameScore</a>#8ef8ecc0 flags:# edit_message:flags.0?<a href="./type/true.md">true</a> force:flags.1?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> id:<a href="./type/int.md">int</a> user_id:<a href="./type/InputUser.md">InputUser</a> score:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/messages.setInlineGameScore.md">messages.setInlineGameScore</a>#15ad9f64 flags:# edit_message:flags.0?<a href="./type/true.md">true</a> force:flags.1?<a href="./type/true.md">true</a> id:<a href="./type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> user_id:<a href="./type/InputUser.md">InputUser</a> score:<a href="./type/int.md">int</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getGameHighScores.md">messages.getGameHighScores</a>#e822649d peer:<a href="./type/InputPeer.md">InputPeer</a> id:<a href="./type/int.md">int</a> user_id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/messages.HighScores.md">messages.HighScores</a>;
<a href="./method/messages.getInlineGameHighScores.md">messages.getInlineGameHighScores</a>#f635e1b id:<a href="./type/InputBotInlineMessageID.md">InputBotInlineMessageID</a> user_id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/messages.HighScores.md">messages.HighScores</a>;
<a href="./method/messages.getCommonChats.md">messages.getCommonChats</a>#d0a48c4 user_id:<a href="./type/InputUser.md">InputUser</a> max_id:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/messages.Chats.md">messages.Chats</a>;
<a href="./method/messages.getAllChats.md">messages.getAllChats</a>#eba80ff0 except_ids:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.Chats.md">messages.Chats</a>;
<a href="./method/messages.getWebPage.md">messages.getWebPage</a>#32ca8f91 url:<a href="./type/string.md">string</a> hash:<a href="./type/int.md">int</a> = <a href="./type/WebPage.md">WebPage</a>;
<a href="./method/messages.toggleDialogPin.md">messages.toggleDialogPin</a>#3289be6a flags:# pinned:flags.0?<a href="./type/true.md">true</a> peer:<a href="./type/InputPeer.md">InputPeer</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.reorderPinnedDialogs.md">messages.reorderPinnedDialogs</a>#959ff644 flags:# force:flags.0?<a href="./type/true.md">true</a> order:Vector&lt;<a href="./type/InputPeer.md">InputPeer</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.getPinnedDialogs.md">messages.getPinnedDialogs</a>#e254d64e = <a href="./type/messages.PeerDialogs.md">messages.PeerDialogs</a>;
<a href="./method/messages.setBotShippingResults.md">messages.setBotShippingResults</a>#e5f672fa flags:# query_id:<a href="./type/long.md">long</a> error:flags.0?<a href="./type/string.md">string</a> shipping_options:flags.1?Vector&lt;<a href="./type/ShippingOption.md">ShippingOption</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/messages.setBotPrecheckoutResults.md">messages.setBotPrecheckoutResults</a>#9c2dd95 flags:# success:flags.1?<a href="./type/true.md">true</a> query_id:<a href="./type/long.md">long</a> error:flags.0?<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;

<a href="./method/updates.getState.md">updates.getState</a>#edd4882a = <a href="./type/updates.State.md">updates.State</a>;
<a href="./method/updates.getDifference.md">updates.getDifference</a>#25939651 flags:# pts:<a href="./type/int.md">int</a> pts_total_limit:flags.0?<a href="./type/int.md">int</a> date:<a href="./type/int.md">int</a> qts:<a href="./type/int.md">int</a> = <a href="./type/updates.Difference.md">updates.Difference</a>;
<a href="./method/updates.getChannelDifference.md">updates.getChannelDifference</a>#3173d78 flags:# force:flags.0?<a href="./type/true.md">true</a> channel:<a href="./type/InputChannel.md">InputChannel</a> filter:<a href="./type/ChannelMessagesFilter.md">ChannelMessagesFilter</a> pts:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/updates.ChannelDifference.md">updates.ChannelDifference</a>;

<a href="./method/photos.updateProfilePhoto.md">photos.updateProfilePhoto</a>#f0bb5152 id:<a href="./type/InputPhoto.md">InputPhoto</a> = <a href="./type/UserProfilePhoto.md">UserProfilePhoto</a>;
<a href="./method/photos.uploadProfilePhoto.md">photos.uploadProfilePhoto</a>#4f32c098 file:<a href="./type/InputFile.md">InputFile</a> = <a href="./type/photos.Photo.md">photos.Photo</a>;
<a href="./method/photos.deletePhotos.md">photos.deletePhotos</a>#87cf7f2f id:Vector&lt;<a href="./type/InputPhoto.md">InputPhoto</a>&gt; = Vector&lt;<a href="./type/long.md">long</a>&gt;;
<a href="./method/photos.getUserPhotos.md">photos.getUserPhotos</a>#91cd32a8 user_id:<a href="./type/InputUser.md">InputUser</a> offset:<a href="./type/int.md">int</a> max_id:<a href="./type/long.md">long</a> limit:<a href="./type/int.md">int</a> = <a href="./type/photos.Photos.md">photos.Photos</a>;

<a href="./method/upload.saveFilePart.md">upload.saveFilePart</a>#b304a621 file_id:<a href="./type/long.md">long</a> file_part:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/upload.getFile.md">upload.getFile</a>#e3a6cfb5 location:<a href="./type/InputFileLocation.md">InputFileLocation</a> offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/upload.File.md">upload.File</a>;
<a href="./method/upload.saveBigFilePart.md">upload.saveBigFilePart</a>#de7b673d file_id:<a href="./type/long.md">long</a> file_part:<a href="./type/int.md">int</a> file_total_parts:<a href="./type/int.md">int</a> bytes:<a href="./type/bytes.md">bytes</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/upload.getWebFile.md">upload.getWebFile</a>#24e6818d location:<a href="./type/InputWebFileLocation.md">InputWebFileLocation</a> offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/upload.WebFile.md">upload.WebFile</a>;
<a href="./method/upload.getCdnFile.md">upload.getCdnFile</a>#2000bcc3 file_token:<a href="./type/bytes.md">bytes</a> offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/upload.CdnFile.md">upload.CdnFile</a>;
<a href="./method/upload.reuploadCdnFile.md">upload.reuploadCdnFile</a>#2e7a2020 file_token:<a href="./type/bytes.md">bytes</a> request_token:<a href="./type/bytes.md">bytes</a> = <a href="./type/Bool.md">Bool</a>;

<a href="./method/help.getConfig.md">help.getConfig</a>#c4f9186b = <a href="./type/Config.md">Config</a>;
<a href="./method/help.getNearestDc.md">help.getNearestDc</a>#1fb33026 = <a href="./type/NearestDc.md">NearestDc</a>;
<a href="./method/help.getAppUpdate.md">help.getAppUpdate</a>#ae2de196 = <a href="./type/help.AppUpdate.md">help.AppUpdate</a>;
<a href="./method/help.saveAppLog.md">help.saveAppLog</a>#6f02f748 events:Vector&lt;<a href="./type/InputAppEvent.md">InputAppEvent</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/help.getInviteText.md">help.getInviteText</a>#4d392343 = <a href="./type/help.InviteText.md">help.InviteText</a>;
<a href="./method/help.getSupport.md">help.getSupport</a>#9cdf08cd = <a href="./type/help.Support.md">help.Support</a>;
<a href="./method/help.getAppChangelog.md">help.getAppChangelog</a>#9010ef6f prev_app_version:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/help.getTermsOfService.md">help.getTermsOfService</a>#350170f3 = <a href="./type/help.TermsOfService.md">help.TermsOfService</a>;
<a href="./method/help.setBotUpdatesStatus.md">help.setBotUpdatesStatus</a>#ec22cfcd pending_updates_count:<a href="./type/int.md">int</a> message:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/help.getCdnConfig.md">help.getCdnConfig</a>#52029342 = <a href="./type/CdnConfig.md">CdnConfig</a>;

<a href="./method/channels.readHistory.md">channels.readHistory</a>#cc104937 channel:<a href="./type/InputChannel.md">InputChannel</a> max_id:<a href="./type/int.md">int</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/channels.deleteMessages.md">channels.deleteMessages</a>#84c1fd4e channel:<a href="./type/InputChannel.md">InputChannel</a> id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.AffectedMessages.md">messages.AffectedMessages</a>;
<a href="./method/channels.deleteUserHistory.md">channels.deleteUserHistory</a>#d10dd71b channel:<a href="./type/InputChannel.md">InputChannel</a> user_id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/messages.AffectedHistory.md">messages.AffectedHistory</a>;
<a href="./method/channels.reportSpam.md">channels.reportSpam</a>#fe087810 channel:<a href="./type/InputChannel.md">InputChannel</a> user_id:<a href="./type/InputUser.md">InputUser</a> id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/Bool.md">Bool</a>;
<a href="./method/channels.getMessages.md">channels.getMessages</a>#93d7b347 channel:<a href="./type/InputChannel.md">InputChannel</a> id:Vector&lt;<a href="./type/int.md">int</a>&gt; = <a href="./type/messages.Messages.md">messages.Messages</a>;
<a href="./method/channels.getParticipants.md">channels.getParticipants</a>#24d98f92 channel:<a href="./type/InputChannel.md">InputChannel</a> filter:<a href="./type/ChannelParticipantsFilter.md">ChannelParticipantsFilter</a> offset:<a href="./type/int.md">int</a> limit:<a href="./type/int.md">int</a> = <a href="./type/channels.ChannelParticipants.md">channels.ChannelParticipants</a>;
<a href="./method/channels.getParticipant.md">channels.getParticipant</a>#546dd7a6 channel:<a href="./type/InputChannel.md">InputChannel</a> user_id:<a href="./type/InputUser.md">InputUser</a> = <a href="./type/channels.ChannelParticipant.md">channels.ChannelParticipant</a>;
<a href="./method/channels.getChannels.md">channels.getChannels</a>#a7f6bbb id:Vector&lt;<a href="./type/InputChannel.md">InputChannel</a>&gt; = <a href="./type/messages.Chats.md">messages.Chats</a>;
<a href="./method/channels.getFullChannel.md">channels.getFullChannel</a>#8736a09 channel:<a href="./type/InputChannel.md">InputChannel</a> = <a href="./type/messages.ChatFull.md">messages.ChatFull</a>;
<a href="./method/channels.createChannel.md">channels.createChannel</a>#f4893d7f flags:# broadcast:flags.0?<a href="./type/true.md">true</a> megagroup:flags.1?<a href="./type/true.md">true</a> title:<a href="./type/string.md">string</a> about:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.editAbout.md">channels.editAbout</a>#13e27f1e channel:<a href="./type/InputChannel.md">InputChannel</a> about:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/channels.editAdmin.md">channels.editAdmin</a>#eb7611d0 channel:<a href="./type/InputChannel.md">InputChannel</a> user_id:<a href="./type/InputUser.md">InputUser</a> role:<a href="./type/ChannelParticipantRole.md">ChannelParticipantRole</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.editTitle.md">channels.editTitle</a>#566decd0 channel:<a href="./type/InputChannel.md">InputChannel</a> title:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.editPhoto.md">channels.editPhoto</a>#f12e57c9 channel:<a href="./type/InputChannel.md">InputChannel</a> photo:<a href="./type/InputChatPhoto.md">InputChatPhoto</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.checkUsername.md">channels.checkUsername</a>#10e6bd2c channel:<a href="./type/InputChannel.md">InputChannel</a> username:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/channels.updateUsername.md">channels.updateUsername</a>#3514b3de channel:<a href="./type/InputChannel.md">InputChannel</a> username:<a href="./type/string.md">string</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/channels.joinChannel.md">channels.joinChannel</a>#24b524c5 channel:<a href="./type/InputChannel.md">InputChannel</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.leaveChannel.md">channels.leaveChannel</a>#f836aa95 channel:<a href="./type/InputChannel.md">InputChannel</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.inviteToChannel.md">channels.inviteToChannel</a>#199f3a6c channel:<a href="./type/InputChannel.md">InputChannel</a> users:Vector&lt;<a href="./type/InputUser.md">InputUser</a>&gt; = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.kickFromChannel.md">channels.kickFromChannel</a>#a672de14 channel:<a href="./type/InputChannel.md">InputChannel</a> user_id:<a href="./type/InputUser.md">InputUser</a> kicked:<a href="./type/Bool.md">Bool</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.exportInvite.md">channels.exportInvite</a>#c7560885 channel:<a href="./type/InputChannel.md">InputChannel</a> = <a href="./type/ExportedChatInvite.md">ExportedChatInvite</a>;
<a href="./method/channels.deleteChannel.md">channels.deleteChannel</a>#c0111fe3 channel:<a href="./type/InputChannel.md">InputChannel</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.toggleInvites.md">channels.toggleInvites</a>#49609307 channel:<a href="./type/InputChannel.md">InputChannel</a> enabled:<a href="./type/Bool.md">Bool</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.exportMessageLink.md">channels.exportMessageLink</a>#c846d22d channel:<a href="./type/InputChannel.md">InputChannel</a> id:<a href="./type/int.md">int</a> = <a href="./type/ExportedMessageLink.md">ExportedMessageLink</a>;
<a href="./method/channels.toggleSignatures.md">channels.toggleSignatures</a>#1f69b606 channel:<a href="./type/InputChannel.md">InputChannel</a> enabled:<a href="./type/Bool.md">Bool</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.updatePinnedMessage.md">channels.updatePinnedMessage</a>#a72ded52 flags:# silent:flags.0?<a href="./type/true.md">true</a> channel:<a href="./type/InputChannel.md">InputChannel</a> id:<a href="./type/int.md">int</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/channels.getAdminedPublicChannels.md">channels.getAdminedPublicChannels</a>#8d8d82d7 = <a href="./type/messages.Chats.md">messages.Chats</a>;

<a href="./method/bots.sendCustomRequest.md">bots.sendCustomRequest</a>#aa2769ed custom_method:<a href="./type/string.md">string</a> params:<a href="./type/DataJSON.md">DataJSON</a> = <a href="./type/DataJSON.md">DataJSON</a>;
<a href="./method/bots.answerWebhookJSONQuery.md">bots.answerWebhookJSONQuery</a>#e6213f4d query_id:<a href="./type/long.md">long</a> data:<a href="./type/DataJSON.md">DataJSON</a> = <a href="./type/Bool.md">Bool</a>;

<a href="./method/payments.getPaymentForm.md">payments.getPaymentForm</a>#99f09745 msg_id:<a href="./type/int.md">int</a> = <a href="./type/payments.PaymentForm.md">payments.PaymentForm</a>;
<a href="./method/payments.getPaymentReceipt.md">payments.getPaymentReceipt</a>#a092a980 msg_id:<a href="./type/int.md">int</a> = <a href="./type/payments.PaymentReceipt.md">payments.PaymentReceipt</a>;
<a href="./method/payments.validateRequestedInfo.md">payments.validateRequestedInfo</a>#770a8e74 flags:# save:flags.0?<a href="./type/true.md">true</a> msg_id:<a href="./type/int.md">int</a> info:<a href="./type/PaymentRequestedInfo.md">PaymentRequestedInfo</a> = <a href="./type/payments.ValidatedRequestedInfo.md">payments.ValidatedRequestedInfo</a>;
<a href="./method/payments.sendPaymentForm.md">payments.sendPaymentForm</a>#2b8879b3 flags:# msg_id:<a href="./type/int.md">int</a> requested_info_id:flags.0?<a href="./type/string.md">string</a> shipping_option_id:flags.1?<a href="./type/string.md">string</a> credentials:<a href="./type/InputPaymentCredentials.md">InputPaymentCredentials</a> = <a href="./type/payments.PaymentResult.md">payments.PaymentResult</a>;
<a href="./method/payments.getSavedInfo.md">payments.getSavedInfo</a>#227d824b = <a href="./type/payments.SavedInfo.md">payments.SavedInfo</a>;
<a href="./method/payments.clearSavedInfo.md">payments.clearSavedInfo</a>#d83d70c1 flags:# credentials:flags.0?<a href="./type/true.md">true</a> info:flags.1?<a href="./type/true.md">true</a> = <a href="./type/Bool.md">Bool</a>;

<a href="./method/phone.getCallConfig.md">phone.getCallConfig</a>#55451fa9 = <a href="./type/DataJSON.md">DataJSON</a>;
<a href="./method/phone.requestCall.md">phone.requestCall</a>#5b95b3d4 user_id:<a href="./type/InputUser.md">InputUser</a> random_id:<a href="./type/int.md">int</a> g_a_hash:<a href="./type/bytes.md">bytes</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> = <a href="./type/phone.PhoneCall.md">phone.PhoneCall</a>;
<a href="./method/phone.acceptCall.md">phone.acceptCall</a>#3bd2b4a0 peer:<a href="./type/InputPhoneCall.md">InputPhoneCall</a> g_b:<a href="./type/bytes.md">bytes</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> = <a href="./type/phone.PhoneCall.md">phone.PhoneCall</a>;
<a href="./method/phone.confirmCall.md">phone.confirmCall</a>#2efe1722 peer:<a href="./type/InputPhoneCall.md">InputPhoneCall</a> g_a:<a href="./type/bytes.md">bytes</a> key_fingerprint:<a href="./type/long.md">long</a> protocol:<a href="./type/PhoneCallProtocol.md">PhoneCallProtocol</a> = <a href="./type/phone.PhoneCall.md">phone.PhoneCall</a>;
<a href="./method/phone.receivedCall.md">phone.receivedCall</a>#17d54f61 peer:<a href="./type/InputPhoneCall.md">InputPhoneCall</a> = <a href="./type/Bool.md">Bool</a>;
<a href="./method/phone.discardCall.md">phone.discardCall</a>#78d413a6 peer:<a href="./type/InputPhoneCall.md">InputPhoneCall</a> duration:<a href="./type/int.md">int</a> reason:<a href="./type/PhoneCallDiscardReason.md">PhoneCallDiscardReason</a> connection_id:<a href="./type/long.md">long</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/phone.setCallRating.md">phone.setCallRating</a>#1c536a34 peer:<a href="./type/InputPhoneCall.md">InputPhoneCall</a> rating:<a href="./type/int.md">int</a> comment:<a href="./type/string.md">string</a> = <a href="./type/Updates.md">Updates</a>;
<a href="./method/phone.saveCallDebug.md">phone.saveCallDebug</a>#277add7e peer:<a href="./type/InputPhoneCall.md">InputPhoneCall</a> debug:<a href="./type/DataJSON.md">DataJSON</a> = <a href="./type/Bool.md">Bool</a>;

// LAYER 66

</pre>
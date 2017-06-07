# User

Object defines a user.

<pre>
<a href="../constructor/userEmpty">userEmpty</a>#200250ba id:<a href="../type/int.md">int</a> = <a href="../type/User.md">User</a>;
<a href="../constructor/user">user</a>#2e13f4c3 flags:<a href="../type/#.md">#</a> self:flags.10?<a href="../type/true.md">true</a> contact:flags.11?<a href="../type/true.md">true</a> mutual_contact:flags.12?<a href="../type/true.md">true</a> deleted:flags.13?<a href="../type/true.md">true</a> bot:flags.14?<a href="../type/true.md">true</a> bot_chat_history:flags.15?<a href="../type/true.md">true</a> bot_nochats:flags.16?<a href="../type/true.md">true</a> verified:flags.17?<a href="../type/true.md">true</a> restricted:flags.18?<a href="../type/true.md">true</a> min:flags.20?<a href="../type/true.md">true</a> bot_inline_geo:flags.21?<a href="../type/true.md">true</a> id:<a href="../type/int.md">int</a> access_hash:flags.0?<a href="../type/long.md">long</a> first_name:flags.1?<a href="../type/string.md">string</a> last_name:flags.2?<a href="../type/string.md">string</a> username:flags.3?<a href="../type/string.md">string</a> phone:flags.4?<a href="../type/string.md">string</a> photo:flags.5?<a href="../type/UserProfilePhoto.md">UserProfilePhoto</a> status:flags.6?<a href="../type/UserStatus.md">UserStatus</a> bot_info_version:flags.14?<a href="../type/int.md">int</a> restriction_reason:flags.18?<a href="../type/string.md">string</a> bot_inline_placeholder:flags.19?<a href="../type/string.md">string</a> lang_code:flags.22?<a href="../type/string.md">string</a> = <a href="../type/User.md">User</a>;

---functions---
<a href="../method/account.updateProfile">account.updateProfile</a>#78515775 flags:<a href="../type/#.md">#</a> first_name:flags.0?<a href="../type/string.md">string</a> last_name:flags.1?<a href="../type/string.md">string</a> about:flags.2?<a href="../type/string.md">string</a> = <a href="../type/User.md">User</a>;
<a href="../method/account.updateUsername">account.updateUsername</a>#3e0bdd7c username:<a href="../type/string.md">string</a> = <a href="../type/User.md">User</a>;
<a href="../method/account.changePhone">account.changePhone</a>#70c32edb phone_number:<a href="../type/string.md">string</a> phone_code_hash:<a href="../type/string.md">string</a> phone_code:<a href="../type/string.md">string</a> = <a href="../type/User.md">User</a>;
<a href="../method/users.getUsers">users.getUsers</a>#d91a548 id:Vector&lt;<a href="../type/InputUser.md">InputUser</a>&gt; = Vector&lt;<a href="../type/User.md">User</a>&gt;;
<a href="../method/contacts.importCard">contacts.importCard</a>#4fe196fe export_card:Vector&lt;<a href="../type/int.md">int</a>&gt; = <a href="../type/User.md">User</a>;
</pre>

## Constructors

| Name | Description |
|------|-------------|
| [userEmpty](../constructor/userEmpty.md) | Empty constructor, non-existent user. |
| [user](../constructor/user.md) | The data of a user. |

## Methods

| Name | Description |
|------|-------------|
| [account.updateProfile](../method/account.updateProfile.md) | Sample Description |
| [account.updateUsername](../method/account.updateUsername.md) | Sample Description |
| [account.changePhone](../method/account.changePhone.md) | Sample Description |
| [users.getUsers](../method/users.getUsers.md) | Sample Description |
| [contacts.importCard](../method/contacts.importCard.md) | Sample Description |

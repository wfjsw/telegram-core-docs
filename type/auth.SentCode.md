# auth.SentCode

Sample Description

<pre>
<a href="../constructor/auth.sentCode">auth.sentCode</a>#5e002502 flags:undefined<a href="../type/#.md">#</a> phone_registered:flags.0?<a href="../type/true.md">true</a> type:undefined<a href="../type/auth.SentCodeType.md">auth.SentCodeType</a> phone_code_hash:undefined<a href="../type/string.md">string</a> next_type:flags.1?<a href="../type/auth.CodeType.md">auth.CodeType</a> timeout:flags.2?<a href="../type/int.md">int</a> = undefined<a href="../type/auth.SentCode.md">auth.SentCode</a>;

---functions---
<a href="../method/auth.sendCode">auth.sendCode</a>#86aef0ec flags:undefined<a href="../type/#.md">#</a> allow_flashcall:flags.0?<a href="../type/true.md">true</a> phone_number:undefined<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> api_id:undefined<a href="../type/int.md">int</a> api_hash:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/auth.resendCode">auth.resendCode</a>#3ef1a9bf phone_number:undefined<a href="../type/string.md">string</a> phone_code_hash:undefined<a href="../type/string.md">string</a> = undefined<a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/account.sendChangePhoneCode">account.sendChangePhoneCode</a>#8e57deb flags:undefined<a href="../type/#.md">#</a> allow_flashcall:flags.0?<a href="../type/true.md">true</a> phone_number:undefined<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/account.sendConfirmPhoneCode">account.sendConfirmPhoneCode</a>#1516d7bd flags:undefined<a href="../type/#.md">#</a> allow_flashcall:flags.0?<a href="../type/true.md">true</a> hash:undefined<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> = undefined<a href="../type/auth.SentCode.md">auth.SentCode</a>;

</pre>

## Constructors

| Name | Description |
|------|-------------|
| [auth.sentCode](../constructor/auth.sentCode.md) | Sample Description |

## Methods

| Name | Description |
|------|-------------|
| [auth.sendCode](../method/auth.sendCode.md) | Sample Description |
| [auth.resendCode](../method/auth.resendCode.md) | Sample Description |
| [account.sendChangePhoneCode](../method/account.sendChangePhoneCode.md) | Sample Description |
| [account.sendConfirmPhoneCode](../method/account.sendConfirmPhoneCode.md) | Sample Description |

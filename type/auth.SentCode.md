# auth.SentCode

Sample Description

<pre>
<a href="../constructor/auth.sentCode.md">auth.sentCode</a>#5e002502 flags:<a href="../type/#.md">#</a> phone_registered:flags.0?<a href="../type/true.md">true</a> type:<a href="../type/auth.SentCodeType.md">auth.SentCodeType</a> phone_code_hash:<a href="../type/string.md">string</a> next_type:flags.1?<a href="../type/auth.CodeType.md">auth.CodeType</a> timeout:flags.2?<a href="../type/int.md">int</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;

---functions---
<a href="../method/auth.sendCode.md">auth.sendCode</a>#86aef0ec flags:<a href="../type/#.md">#</a> allow_flashcall:flags.0?<a href="../type/true.md">true</a> phone_number:<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> api_id:<a href="../type/int.md">int</a> api_hash:<a href="../type/string.md">string</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/auth.resendCode.md">auth.resendCode</a>#3ef1a9bf phone_number:<a href="../type/string.md">string</a> phone_code_hash:<a href="../type/string.md">string</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/account.sendChangePhoneCode.md">account.sendChangePhoneCode</a>#8e57deb flags:<a href="../type/#.md">#</a> allow_flashcall:flags.0?<a href="../type/true.md">true</a> phone_number:<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/account.sendConfirmPhoneCode.md">account.sendConfirmPhoneCode</a>#1516d7bd flags:<a href="../type/#.md">#</a> allow_flashcall:flags.0?<a href="../type/true.md">true</a> hash:<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
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

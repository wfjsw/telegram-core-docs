# auth.SentCode

Sample Description

<pre>
<a href="../constructor/auth.sentCode">auth.sentCode</a>#5e002502 flags:<a href="../type/#.md">#</a> phone_registered:<a href="../type/flags.0?true.md">flags.0?true</a> type:<a href="../type/auth.SentCodeType.md">auth.SentCodeType</a> phone_code_hash:<a href="../type/string.md">string</a> next_type:<a href="../type/flags.1?auth.CodeType.md">flags.1?auth.CodeType</a> timeout:<a href="../type/flags.2?int.md">flags.2?int</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;

---functions---
<a href="../method/auth.sendCode">auth.sendCode</a>#86aef0ec flags:<a href="../type/#.md">#</a> allow_flashcall:<a href="../type/flags.0?true.md">flags.0?true</a> phone_number:<a href="../type/string.md">string</a> current_number:<a href="../type/flags.0?Bool.md">flags.0?Bool</a> api_id:<a href="../type/int.md">int</a> api_hash:<a href="../type/string.md">string</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/auth.resendCode">auth.resendCode</a>#3ef1a9bf phone_number:<a href="../type/string.md">string</a> phone_code_hash:<a href="../type/string.md">string</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/account.sendChangePhoneCode">account.sendChangePhoneCode</a>#8e57deb flags:<a href="../type/#.md">#</a> allow_flashcall:<a href="../type/flags.0?true.md">flags.0?true</a> phone_number:<a href="../type/string.md">string</a> current_number:<a href="../type/flags.0?Bool.md">flags.0?Bool</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
<a href="../method/account.sendConfirmPhoneCode">account.sendConfirmPhoneCode</a>#1516d7bd flags:<a href="../type/#.md">#</a> allow_flashcall:<a href="../type/flags.0?true.md">flags.0?true</a> hash:<a href="../type/string.md">string</a> current_number:<a href="../type/flags.0?Bool.md">flags.0?Bool</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;

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

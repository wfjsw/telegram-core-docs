# account.sendChangePhoneCode

Sample Description

<pre>
<a href="../constructor/auth.sentCode.md">auth.sentCode</a>#5e002502 flags:# phone_registered:flags.0?<a href="../type/true.md">true</a> type:<a href="../type/auth.SentCodeType.md">auth.SentCodeType</a> phone_code_hash:<a href="../type/string.md">string</a> next_type:flags.1?<a href="../type/auth.CodeType.md">auth.CodeType</a> timeout:flags.2?<a href="../type/int.md">int</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;

---functions---
<a href="../method/account.sendChangePhoneCode.md">account.sendChangePhoneCode</a>#8e57deb flags:# allow_flashcall:flags.0?<a href="../type/true.md">true</a> phone_number:<a href="../type/string.md">string</a> current_number:flags.0?<a href="../type/Bool.md">Bool</a> = <a href="../type/auth.SentCode.md">auth.SentCode</a>;
</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **flags** | # | Param description |
| **allow_flashcall** | flags.0?<a href="../type/true.md">true</a> | Param description |
| **phone_number** | <a href="../type/string.md">string</a> | Param description |
| **current_number** | flags.0?<a href="../type/Bool.md">Bool</a> | Param description |

## Result

<a href="../type/auth.SentCode.md">auth.SentCode</a>


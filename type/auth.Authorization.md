# auth.Authorization

Sample Description

<pre>
<a href="../constructor/auth.authorization">auth.authorization</a>#cd050916 flags:<a href="../type/#.md">#</a> tmp_sessions:<a href="../type/flags.0?int.md">flags.0?int</a> user:<a href="../type/User.md">User</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;

---functions---
<a href="../method/auth.signUp">auth.signUp</a>#1b067634 phone_number:<a href="../type/string.md">string</a> phone_code_hash:<a href="../type/string.md">string</a> phone_code:<a href="../type/string.md">string</a> first_name:<a href="../type/string.md">string</a> last_name:<a href="../type/string.md">string</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;
<a href="../method/auth.signIn">auth.signIn</a>#bcd51581 phone_number:<a href="../type/string.md">string</a> phone_code_hash:<a href="../type/string.md">string</a> phone_code:<a href="../type/string.md">string</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;
<a href="../method/auth.importAuthorization">auth.importAuthorization</a>#e3ef9613 id:<a href="../type/int.md">int</a> bytes:<a href="../type/bytes.md">bytes</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;
<a href="../method/auth.importBotAuthorization">auth.importBotAuthorization</a>#67a3ff2c flags:<a href="../type/int.md">int</a> api_id:<a href="../type/int.md">int</a> api_hash:<a href="../type/string.md">string</a> bot_auth_token:<a href="../type/string.md">string</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;
<a href="../method/auth.checkPassword">auth.checkPassword</a>#a63011e password_hash:<a href="../type/bytes.md">bytes</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;
<a href="../method/auth.recoverPassword">auth.recoverPassword</a>#4ea56e92 code:<a href="../type/string.md">string</a> = <a href="../type/auth.Authorization.md">auth.Authorization</a>;

</pre>

## Constructors

| Name | Description |
|------|-------------|
| [auth.authorization](../constructor/auth.authorization.md) | Sample Description |

## Methods

| Name | Description |
|------|-------------|
| [auth.signUp](../method/auth.signUp.md) | Sample Description |
| [auth.signIn](../method/auth.signIn.md) | Sample Description |
| [auth.importAuthorization](../method/auth.importAuthorization.md) | Sample Description |
| [auth.importBotAuthorization](../method/auth.importBotAuthorization.md) | Sample Description |
| [auth.checkPassword](../method/auth.checkPassword.md) | Sample Description |
| [auth.recoverPassword](../method/auth.recoverPassword.md) | Sample Description |
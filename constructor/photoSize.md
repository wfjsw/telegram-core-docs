# photoSize

Image description.

<pre>
<a href="../constructor/photoSize.md">photoSize</a>#77bfb61b type:<a href="../type/string.md">string</a> location:<a href="../type/FileLocation.md">FileLocation</a> w:<a href="../type/int.md">int</a> h:<a href="../type/int.md">int</a> size:<a href="../type/int.md">int</a> = <a href="../type/PhotoSize.md">PhotoSize</a>;</pre>
## Parameters

| Name | Type | Description |
|------|:----:|-------------|
| **type** | <a href="../type/string.md">string</a> | Thumbnail type |
| **location** | <a href="../type/FileLocation.md">FileLocation</a> | File location |
| **w** | <a href="../type/int.md">int</a> | Image width |
| **h** | <a href="../type/int.md">int</a> | Image height |
| **size** | <a href="../type/int.md">int</a> | File size |

## Thumbnail type and its sizes

| Type | Image filter | Size limits, px |
|------|--------------|-----------------|
|`s`   |box           |100x100          |
|`m`   |box           |320x320          |
|`x`   |box           |800x800          |
|`y`   |box           |1280x1280        |
|`w`   |box           |2560x2560        |
|`a`   |crop          |160x160          |
|`b`   |crop          |320x320          |
|`c`   |crop          |640x640          |
|`d`   |crop          |1280x1280        |

## Type

<a href="../type/PhotoSize.md">PhotoSize</a>

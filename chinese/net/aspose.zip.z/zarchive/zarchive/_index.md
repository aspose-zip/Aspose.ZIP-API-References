---
title: ZArchive.ZArchive
second_title: Aspose.ZIP for .NET API 参考
description: ZArchive 构造函数. 初始化一个新的实例ZArchive准备压缩的类.
type: docs
weight: 10
url: /zh/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

初始化一个新的实例[`ZArchive`](../)准备压缩的类.

```csharp
public ZArchive()
```

### 也可以看看

* class [ZArchive](../)
* 命名空间 [Aspose.Zip.Z](../../zarchive/)
* 部件 [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

初始化一个新的实例[`ZArchive`](../)准备解压的类.

```csharp
public ZArchive(Stream source)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| source | Stream | 存档的来源。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *source*不可搜索。 |
| ArgumentNullException | *source*一片空白。 |

### 评论

此构造函数不解压缩。看[`Extract`](../extract/)解压方法.

### 也可以看看

* class [ZArchive](../)
* 命名空间 [Aspose.Zip.Z](../../zarchive/)
* 部件 [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

初始化一个新的实例[`ZArchive`](../)准备解压的类.

```csharp
public ZArchive(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档源的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压缩。看[`Extract`](../extract/)解压方法.

### 也可以看看

* class [ZArchive](../)
* 命名空间 [Aspose.Zip.Z](../../zarchive/)
* 部件 [Aspose.Zip](../../../)



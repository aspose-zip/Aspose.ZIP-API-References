---
title: Class License
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.License 班级. 提供许可组件的方法
type: docs
weight: 260
url: /zh/net/aspose.zip/license/
---
## License class

提供许可组件的方法。

```csharp
public class License
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [License](license/)() | 初始化一个新的实例`License`班级。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | 许可组件。 |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | 许可组件。 |

### 例子

在此示例中，将尝试在包含 的文件夹中查找名为 MyLicense.lic 的许可证文件 组件，在包含调用程序集的文件夹中， 在入口程序集的文件夹中，然后在调用程序集的嵌入资源中。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

组件 jar 文件：

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### 也可以看看

* 命名空间 [Aspose.Zip](../../aspose.zip/)
* 部件 [Aspose.Zip](../../)



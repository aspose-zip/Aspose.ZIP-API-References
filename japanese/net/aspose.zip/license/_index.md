---
title: "クラス License"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.License クラス。コンポーネントにライセンスを付与するメソッドを提供します。"
type: docs
weight: 660
url: /ja/net/aspose.zip/license/
---
## License class

コンポーネントをライセンスするためのメソッドを提供します。

```csharp
public sealed class License
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [License](license/)() | `License` クラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | コンポーネントにライセンスを付与します。 |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | コンポーネントにライセンスを付与します。 |

## 例

この例では、コンポーネントが含まれるフォルダー、呼び出しアセンブリが含まれるフォルダー、エントリ アセンブリのフォルダー、そして呼び出しアセンブリの埋め込みリソース内で、MyLicense.lic という名前のライセンス ファイルを検索しようとします。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

コンポーネントの jar ファイル:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### 関連項目

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)



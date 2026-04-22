---
title: Class License
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.License クラス. コンポーネントのライセンスを取得する方法を提供します
type: docs
weight: 260
url: /ja/net/aspose.zip/license/
---
## License class

コンポーネントのライセンスを取得する方法を提供します。

```csharp
public class License
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [License](license/)() | の新しいインスタンスを初期化します`License`クラス。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | コンポーネントのライセンスを取得します。 |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | コンポーネントのライセンスを取得します。 |

### 例

この例では、 を含むフォルダーで MyLicense.lic という名前のライセンス ファイルを見つけようとします。 呼び出しアセンブリを含むフォルダー内のコンポーネント、 エントリ アセンブリのフォルダー内、および呼び出しアセンブリの埋め込みリソース内のコンポーネント.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

コンポーネント jar ファイル:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### 関連項目

* 名前空間 [Aspose.Zip](../../aspose.zip/)
* 組み立て [Aspose.Zip](../../)



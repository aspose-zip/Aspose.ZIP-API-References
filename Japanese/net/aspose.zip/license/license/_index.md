---
title: License.License
second_title: Aspose.ZIP for .NET API リファレンス
description: License コンストラクタ. の新しいインスタンスを初期化しますLicenseクラス
type: docs
weight: 10
url: /ja/net/aspose.zip/license/license/
---
## License constructor

の新しいインスタンスを初期化します[`License`](../)クラス。

```csharp
public License()
```

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

* class [License](../)
* 名前空間 [Aspose.Zip](../../license/)
* 組み立て [Aspose.Zip](../../../)



---
title: "License.License"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "License コンストラクタ。License クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip/license/license/
---
## License constructor

[`License`](../) クラスの新しいインスタンスを初期化します。

```csharp
public License()
```

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

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)



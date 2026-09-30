---
title: "License.SetLicense"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "License メソッド。コンポーネントにライセンスを付与します"
type: docs
weight: 20
url: /ja/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

コンポーネントにライセンスを付与します。

```csharp
public void SetLicense(string licenseName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| licenseName | String | 完全または短いファイル名、または埋め込みリソースの名前にできます。空文字列を使用すると評価モードに切り替わります。 |

## 備考

次の場所でライセンスを検索します：

1. 明示的なパス。

2. Aspose コンポーネント アセンブリが含まれるフォルダー。

3. クライアントの呼び出しアセンブリが含まれるフォルダー。

4. エントリ（スタートアップ）アセンブリが含まれるフォルダー。

5. クライアントの呼び出しアセンブリに埋め込まれたリソース。

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. 明示的なパス。

2. クライアントの呼び出しアセンブリに埋め込まれたリソース。

2. Aspose コンポーネント JAR ファイルが含まれるフォルダー。

3. クライアントの呼び出し JAR ファイルが含まれるフォルダー。

## 例

この例では、コンポーネントが含まれるフォルダー、呼び出しアセンブリが含まれるフォルダー、エントリ アセンブリのフォルダー、そして呼び出しアセンブリの埋め込みリソース内で、MyLicense.lic という名前のライセンス ファイルを検索しようとします。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
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

---

## SetLicense(Stream) {#setlicense}

コンポーネントにライセンスを付与します。

```csharp
public void SetLicense(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ライセンスを含むストリーム。 |

## 備考

このメソッドを使用して、ストリームからライセンスをロードします。

## 例

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### 関連項目

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)



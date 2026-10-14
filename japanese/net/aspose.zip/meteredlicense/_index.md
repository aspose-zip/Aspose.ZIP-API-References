---
title: "クラス MeteredLicense"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.MeteredLicense クラス。メーターキーを設定するメソッドを提供します。"
type: docs
weight: 760
url: /ja/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

メータリングキーを設定するためのメソッドを提供します。

```csharp
public class MeteredLicense
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | デフォルト コンストラクタです。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [ResetMeteredKey](../../aspose.zip/meteredlicense/resetmeteredkey/)() | 以前に設定されたライセンスを削除します。 |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | メーターの公開キーと秘密キーを設定します。 |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | 消費クレジットを取得します。 |
| static [GetConsumptionQuantity](../../aspose.zip/meteredlicense/getconsumptionquantity/)() | 消費ファイルサイズを取得します。 |

## 例

この例では、メーターの公開キーと秘密キーを設定しようとします。

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

コンポーネントの jar ファイル:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### 関連項目

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)



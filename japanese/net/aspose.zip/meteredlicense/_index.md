---
title: Class MeteredLicense
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.MeteredLicense クラス. メータリング キーを設定するメソッドを提供します
type: docs
weight: 290
url: /ja/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

メータリング キーを設定するメソッドを提供します。

```csharp
public class MeteredLicense
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | このクラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | 従量制の公開鍵と秘密鍵を設定します。 |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | 消費クレジットを取得します。 |

### 備考

重要: 従量制ライセンスでは、自己解凍型の zip アーカイブを作成することはできません.

### 例

この例では、従量制の公開鍵と秘密鍵を設定しようとします。

```csharp
MeteredLicense matered = new MeteredLicense();
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

### 関連項目

* 名前空間 [Aspose.Zip](../../aspose.zip/)
* 組み立て [Aspose.Zip](../../)



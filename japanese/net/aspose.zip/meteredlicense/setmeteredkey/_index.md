---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP for .NET API リファレンス
description: MeteredLicense 方法. 従量制の公開鍵と秘密鍵を設定します
type: docs
weight: 20
url: /ja/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

従量制の公開鍵と秘密鍵を設定します。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| publicKey | String | 公開鍵。 |
| privateKey | String | 秘密鍵。 |

### 備考

従量制ライセンスを購入した場合、アプリ起動時にこの API を呼び出す必要がありますが、通常はこれで十分です。 ただし、常に消費データのアップロードに失敗し、24 時間を超えると、ライセンスは評価ステータスに設定されます. そのような場合を避けるために、定期的にライセンスステータスを確認し、評価ステータスである場合は、この API を再度呼び出す必要があります.

### 関連項目

* class [MeteredLicense](../)
* 名前空間 [Aspose.Zip](../../meteredlicense/)
* 組み立て [Aspose.Zip](../../../)



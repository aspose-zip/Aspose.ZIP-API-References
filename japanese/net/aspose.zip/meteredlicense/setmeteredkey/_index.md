---
title: "MeteredLicense.SetMeteredKey"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "MeteredLicense メソッド。メータードの公開キーと秘密キーを設定します。"
type: docs
weight: 30
url: /ja/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

メーターの公開キーと秘密キーを設定します。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| publicKey | String | 公開キーです。 |
| privateKey | String | 秘密キーです。 |

## 備考

メータードライセンスを購入した場合、この API はアプリケーションの起動時に呼び出す必要があります。通常、これだけで十分です。ただし、メータードが 24 時間以内に使用データのアップロードに失敗した場合、ライセンスは評価版ステータスに設定されます。そのような事態を防ぐため、ライセンスのステータスを定期的に確認し、評価版ステータスである場合は再度この API を呼び出してください。

### 関連項目

* class [MeteredLicense](../)
* namespace [Aspose.Zip](../../meteredlicense/)
* assembly [Aspose.Zip](../../../)



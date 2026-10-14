---
title: "MeteredLicense"
second_title: "Aspose.ZIP for Java API 참조"
description: "계량된 키를 설정하는 메서드를 제공합니다."
type: docs
weight: 92
url: /ko/java/com.aspose.zip/meteredlicense/
---

**Inheritance:**
java.lang.Object
```
public class MeteredLicense
```

계량된 키를 설정하는 메서드를 제공합니다.


이 예제에서는 계량된 공개 및 개인 키를 설정하려고 시도합니다.

```

``````

MeteredLicense metered = new MeteredLicense();
metered.setMeteredKey("PublicKey", "PrivateKey");
 
```

Important: with metered license you cannot compose self-extracting zip archives.
## Constructors

| Constructor | Description |
| --- | --- |
| [MeteredLicense()](#MeteredLicense--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getConsumptionCredit()](#getConsumptionCredit--) | Gets consumption credit. |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Gets consumption file size. |
| [isLicensed()](#isLicensed--) | Checks whether the product is successfully licensed using Metered license. |
| [resetMeteredKey()](#resetMeteredKey--) | Removes previously setup license. |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Sets metered public and private keys. |
### MeteredLicense() {#MeteredLicense--}
```
public MeteredLicense()
```


### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Gets consumption credit.

**Returns:**
java.math.BigDecimal - Returns the number of consumed credit points.
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Gets consumption file size.

**Returns:**
java.math.BigDecimal - Returns the number of consumed bytes.
### isLicensed() {#isLicensed--}
```
public final boolean isLicensed()
```


Checks whether the product is successfully licensed using Metered license.

**Returns:**
boolean - true or false
### resetMeteredKey() {#resetMeteredKey--}
```
public final void resetMeteredKey()
```


Removes previously setup license.

### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Sets metered public and private keys.

If you purchase metered license, this API should be called on application startup, normally, this is enough. However, if metered fails to upload consumption data during 24 hours period, the license will be set to evaluation status. To avoid such case, you should regularly check the license status If it is evaluation status, call this API again.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | The public key. |
| privateKey | java.lang.String | The private key. |


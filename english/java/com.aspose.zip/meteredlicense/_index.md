---
title: MeteredLicense
second_title: Aspose.ZIP for Java API Reference
description: Provides methods to set metered key.
type: docs
weight: 29
url: /java/com.aspose.zip/meteredlicense/
---

**Inheritance:**
java.lang.Object
```
public class MeteredLicense
```

Provides methods to set metered key.


In this example, an attempt will be made to set metered public and private key.

```

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

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | The public key. |
| privateKey | java.lang.String | The private key.

--------------------

If you purchase metered license, this API should be called on application startup, normally, this is enough. However, if metered fails to upload consumption data during 24 hours period, the license will be set to evaluation status. To avoid such case, you should regularly check the license status If it is evaluation status, call this API again. |


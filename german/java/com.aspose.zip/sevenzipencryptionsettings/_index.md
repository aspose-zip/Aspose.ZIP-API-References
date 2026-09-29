---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Basisklasse für Einstellungen mehrerer 7z-Verschlüsselungsmethoden."
type: docs
weight: 112
url: /de/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Basisklasse für Einstellungen mehrerer 7z-Verschlüsselungsmethoden.

Der AES-256 ist die einzige mögliche Verschlüsselungsmethode für 7z-Archive. Daher ist die [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) die einzige Implementierung.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Gibt einen Wert zurück, der die Header-Verschlüsselung angibt. |
| [getPassword()](#getPassword--) | Gibt das Passwort für Verschlüsselung oder Entschlüsselung zurück. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Setzt einen Wert, der die Header-Verschlüsselung angibt. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Setzt das Passwort für Verschlüsselung oder Entschlüsselung. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Gibt einen Wert zurück, der die Header-Verschlüsselung angibt.

Diese Einstellung entspricht dem Schalter `-mhe=on` des 7‑Zip‑Tools. Derzeit ist sie mit Header-Kompression inkompatibel.

**Returns:**
boolean - ein Wert, der die Header-Verschlüsselung angibt
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gibt das Passwort für Verschlüsselung oder Entschlüsselung zurück.

**Returns:**
java.lang.String - Passwort für Verschlüsselung oder Entschlüsselung
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Setzt einen Wert, der die Header-Verschlüsselung angibt.

Diese Einstellung entspricht dem Schalter `-mhe=on` des 7‑Zip‑Tools. Derzeit ist sie mit Header-Kompression inkompatibel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der die Header-Verschlüsselung angibt |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Setzt das Passwort für Verschlüsselung oder Entschlüsselung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Passwort für Verschlüsselung oder Entschlüsselung |


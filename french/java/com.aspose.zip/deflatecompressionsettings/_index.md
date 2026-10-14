---
title: "DeflateCompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la compression Deflate dans une archive ZIP."
type: docs
weight: 59
url: /fr/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Paramètres pour la compression Deflate dans une archive ZIP.

Deflate est un algorithme de compression de données sans perte qui utilise une combinaison de l'algorithme LZ77 et du codage Huffman.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Initialise une nouvelle instance de la classe [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Initialise une nouvelle instance de la classe [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```




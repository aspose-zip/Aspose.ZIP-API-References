---
title: "AppleArchive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo AppleArchive. Salva l'archivio nello stream fornito."
type: docs
weight: 90
url: /it/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream output)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Stream di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato. |
| ArgumentNullException | *output* è `null`. |
| ArgumentException | *output* non è scrivibile. |
| ArgumentOutOfRangeException | La dimensione del blocco LZ4 o Zlib configurata non è positiva. |
| NotSupportedException | Le impostazioni di compressione sono mancanti o non supportate, la composizione diretta utilizza uno stream non ricercabile, oppure la dimensione della voce/archivio supera i limiti attuali di Apple Archive. |

## Osservazioni

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Vedi anche

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Salva l'archivio in un file di destinazione fornito.

```csharp
public void Save(string destinationFileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato. |
| ArgumentException | *destinationFileName* non è valido. |
| ArgumentNullException | *destinationFileName* è `null`. |
| ArgumentOutOfRangeException | La dimensione del blocco LZ4 o Zlib configurata non è positiva. |
| NotSupportedException | Le impostazioni di compressione sono mancanti o non supportate, la composizione diretta utilizza uno stream non ricercabile, oppure la dimensione della voce/archivio supera i limiti attuali di Apple Archive. |

### Vedi anche

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)



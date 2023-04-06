---
title: SevenZipArchive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipArchive metodo. Salva larchivio 7z nello stream fornito.
type: docs
weight: 80
url: /it/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Salva l'archivio 7z nello stream fornito.

```csharp
public void Save(Stream output)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Flusso di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *output* non supporta la ricerca. |
| ArgumentNullException | *output* è zero. |
| InvalidOperationException | Il codificatore non è riuscito a comprimere i dati. |

### Osservazioni

*output* deve essere ricercabile.

### Esempi

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Guarda anche

* class [SevenZipArchive](../)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationFileName* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*destinationFileName* è negato. |
| PathTooLongException | Il specificato*destinationFileName*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*destinationFileName* contiene i due punti (:) al centro della stringa. |

### Osservazioni

È possibile salvare un archivio nello stesso percorso da cui è stato caricato. Tuttavia, ciò non è consigliato poiché questo approccio utilizza la copia in un file temporaneo.

### Esempi

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Guarda anche

* class [SevenZipArchive](../)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assemblea [Aspose.Zip](../../../)



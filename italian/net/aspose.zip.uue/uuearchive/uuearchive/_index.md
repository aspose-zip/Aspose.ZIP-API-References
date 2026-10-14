---
title: "UueArchive.UueArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "UueArchive constructor. Inizializza una nuova istanza della classe UueArchive preparata per la codifica"
type: docs
weight: 10
url: /it/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Inizializza una nuova istanza della classe [`UueArchive`](../) preparata per la codifica.

```csharp
public UueArchive()
```

## Esempi

Il seguente esempio mostra come uuencode un file.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Vedi anche

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Inizializza una nuova istanza della classe [`UueArchive`](../) preparata per la decodifica.

```csharp
public UueArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La sorgente dell'archivio. |

## Osservazioni

Questo costruttore non decodifica. Vedi il metodo [`Open`](../open/) per decomprimere.

## Esempi

Apri un archivio da uno stream ed estrailo in un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Vedi anche

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Inizializza una nuova istanza della classe [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso al file di archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| FileNotFoundException | Il file non è stato trovato. |
| IOException | Il file è già aperto. |

## Osservazioni

Questo costruttore non decomprime. Vedi il metodo [`Open`](../open/) per decomprimere.

## Esempi

Apri un archivio da file per percorso e decodificalo in un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Vedi anche

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)



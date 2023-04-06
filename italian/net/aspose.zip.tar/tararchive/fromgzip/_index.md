---
title: TarArchive.FromGZip
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive metodo. Estrae larchivio gzip fornito e componeTarArchive dai dati estratti.
type: docs
weight: 20
url: /it/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Estrae l'archivio gzip fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio gzip viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | La fonte dell'archivio. |

### Valore di ritorno

Un'istanza di[`TarArchive`](../)

### Osservazioni

Il flusso di estrazione GZip non è ricercabile per la natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare un flusso ricercabile sotto il cofano.

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Estrae l'archivio gzip fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio gzip viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromGZip(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di archivio. |

### Valore di ritorno

Un'istanza di[`TarArchive`](../)

### Osservazioni

Il flusso di estrazione GZip non è ricercabile per la natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare un flusso ricercabile sotto il cofano.

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)



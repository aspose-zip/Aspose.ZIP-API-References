---
title: TarArchive.FromLZip
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive metodo. Estrae larchivio lzip fornito e componeTarArchive dai dati estratti.
type: docs
weight: 30
url: /it/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Estrae l'archivio lzip fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio lzip viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | La fonte dell'archivio. |

### Valore di ritorno

Un'istanza di[`TarArchive`](../)

### Osservazioni

Il flusso di estrazione Lzip non è ricercabile per la natura dell'algoritmo di compressione. L'archivio tar fornisce la possibilità di estrarre record arbitrari, quindi deve gestire un flusso ricercabile sotto il cofano.

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Estrae l'archivio lzip fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio lzip viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromLZip(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di archivio. |

### Valore di ritorno

Un'istanza di[`TarArchive`](../)

### Osservazioni

Il flusso di estrazione Lzip non è ricercabile per la natura dell'algoritmo di compressione. L'archivio tar fornisce la possibilità di estrarre record arbitrari, quindi deve gestire un flusso ricercabile sotto il cofano.

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)



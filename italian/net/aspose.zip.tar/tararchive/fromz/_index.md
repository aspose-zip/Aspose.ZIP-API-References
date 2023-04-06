---
title: TarArchive.FromZ
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive metodo. Estrae larchivio in formato Z fornito e componeTarArchive dai dati estratti.
type: docs
weight: 50
url: /it/net/aspose.zip.tar/tararchive/fromz/
---
## FromZ(Stream) {#fromz}

Estrae l'archivio in formato Z fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio Z viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromZ(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | La fonte dell'archivio. |

### Valore di ritorno

Un'istanza di[`TarArchive`](../)

### Osservazioni

L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve gestire un flusso ricercabile sotto il cofano.

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)

---

## FromZ(string) {#fromz_1}

Estrae l'archivio in formato Z fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio Z viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromZ(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di archivio. |

### Valore di ritorno

Un'istanza di[`TarArchive`](../)

### Osservazioni

L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve gestire un flusso ricercabile sotto il cofano.

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)



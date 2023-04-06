---
title: TarArchive.FromXz
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive metodo. Estrae larchivio in formato xz fornito e componeTarArchive dai dati estratti.
type: docs
weight: 40
url: /it/net/aspose.zip.tar/tararchive/fromxz/
---
## FromXz(Stream) {#fromxz}

Estrae l'archivio in formato xz fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio xz viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromXz(Stream source)
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

## FromXz(string) {#fromxz_1}

Estrae l'archivio in formato xz fornito e compone[`TarArchive`](../) dai dati estratti.

Importante: l'archivio xz viene completamente estratto all'interno di questo metodo, il suo contenuto viene conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromXz(string path)
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



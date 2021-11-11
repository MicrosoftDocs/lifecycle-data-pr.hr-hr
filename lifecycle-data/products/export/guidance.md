---
title: Smjernice za izvoz podataka životnog ciklusa
description: Smjernice za izvoz informacija o životnom ciklusu proizvoda
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546763"
---
# <a name="lifecycle-data-export-guidance"></a>Smjernice za izvoz podataka životnog ciklusa
U ovom se dokumentu opisuje kako koristiti datoteku za izvoz proizvoda.

## <a name="query-information"></a>Informacije o upitu
U dokumentu Excel postoje polja koja pomažu u prepoznavanju podataka koji se popunjavaju u tablici proizvoda.

### <a name="end-of-support"></a>Završetak podrške
Vrijednost završetka podrške filtrirat će proizvode prema datumu završetka podrške ili datumima završetka izdanja.

Moguće vrijednosti: Sve (bez primijenjenog filtra), Godina i Raspon.

### <a name="family"></a>Obitelj
Vrijednost linije filtrira proizvode prema nadređenoj razini unutar hijerarhije poznate kao linija.

Moguće vrijednosti: Sve (nije primijenjen filtar), Naziv linije

### <a name="group"></a>Grupa
Vrijednost grupe filtrira proizvode unutar nadređene razine (linije) u određenu grupu.

Moguće vrijednosti: Sve (nije primijenjen filtar), Naziv grupe

## <a name="table-columns"></a>Stupci u tablici
Tablica proizvoda sastoji se od stupaca u kojima se definiraju proizvod, edicije, izdanja i odgovarajući datumi podrške.

> [!NOTE]
> Za svaki proizvod, ediciju i kombinaciju izdanja postojat će redak.

### <a name="product"></a>Proizvod
Naziv proizvoda.

### <a name="edition"></a>Izdanje
Stupac edicije popunjava se kada proizvod sadrži edicije. Kada nema edicije proizvoda, to će polje biti prazno.

### <a name="release"></a>Izdanje
Stupac izdanja popunjava se kada proizvod ima više izdanja.
Kada proizvod ima samo jedno izdanje, to će polje biti prazno.

### <a name="support-policy"></a>Pravila za podršku
U tom se polju definira koja pravila za podršku proizvod slijedi.

Moguće vrijednosti: [Fiksna,](/lifecycle/policies/fixed) [Moderna](/lifecycle/policies/modern), Komponentna

### <a name="start-date"></a>Datum početka
Datum početka podrške za proizvod.

### <a name="mainstream-date"></a>Glavni datum
Kada su pravila za podršku **Fiksna** ili **Komponentna**, to je glavni datum završetka za proizvod.
  
Kada su pravila za podršku **Moderna**, to će biti prazno.

### <a name="extended-end-date"></a>Produženi datum podrške
Kada su pravila za podršku **Fiksna** ili **Komponentna**, to je produženi datum završetka za proizvod.

Kada su pravila za podršku **Moderna**, to će biti prazno.

### <a name="retirement-date"></a>Datum umirovljenja
Kada su pravila za podršku **Fiksna** ili **Komponentna**, to će biti prazno.

Kada su pravila za podršku **Moderna**, to će biti datum umirovljenja proizvoda.

### <a name="release-start-date"></a>Datum početka izdanja
Datum početka podrške za izdanje. Kada proizvod ima samo jedno izdanje, to će polje biti prazno.
 
### <a name="release-end-date"></a>Datum završetka izdanja
Datum završetka podrške za izdanje.
Kada proizvod ima samo jedno izdanje, to će polje biti prazno.

### <a name="docs-url"></a>URL dokumenata
URL na proširenu dokumentaciju.

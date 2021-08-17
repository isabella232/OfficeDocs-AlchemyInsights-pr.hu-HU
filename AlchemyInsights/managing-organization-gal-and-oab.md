---
title: A szervezeti globális címlista és az offline címjegyzék kezelése
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042164"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>A szervezeti globális címlista (GAL) és az offline címjegyzék (OAB) kezelése

A globális címlista (GAL) a szervezet levelezésre alkalmas objektumainak (e-mail fogadására képes bármilyen típusú címzettjeinek) listája. A rendszer mindegyik szervezetben automatikusan létrehoz egy globális címlistát. Létrehozhat további globális címlistákat, ha szeretné szervezet vagy hely szerint különválasztani a felhasználókat, de egy adott felhasználó egyszerre csak egy globális címlistát láthat és használhat.

Egyes levelezőprogramok – például a Windows Outlook – letöltik a globális címlistát offline használatra. Ez a letöltött címlista az offline címjegyzék (OAB). Az Exchange Online-ban egy offline címjegyzék mindössze 8 óránként frissül, és utána az ügyfeleknek le kell tölteniük, hogy frissítsék az offline címjegyzékük helyi példányát. A címzettek mindennemű módosításának először a globális címlistán kell megjelennie, hogy később bekerüljön az offline címjegyzékbe.

Alább felsorolunk néhány, a globális címlistával és az offline címjegyzékkel kapcsolatos gyakori eljárást:

- Számos különböző ok miatt előfordulhat, hogy el szeretne rejteni egyes objektumokat a globális címlistáról. Ehhez tekintse át a [Címzettek elrejtése címlistákról](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists) című témakört.
- Ha testreszabott nézeteket kell biztosítania a szervezet globális címlistájáról a felhasználók meghatározott csoportjai számára, olvassa el a [Címjegyzék-házirendek az Exchange Online-ban](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies) című témakört.
- [Hozzon létre egy globális címlistát az Exchange Online-ban](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), és ismerkedjen meg a globális címlistákra vonatkozó engedélyek használatával, ehhez tekintse át a [Címlisták az Exchange Online-ban](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) című témakört. Felhívjuk a figyelmét arra, hogy új globális címlista létrehozása esetén célszerű lehet egy új offline címjegyzéket is létrehozni. Erről [Az offline címjegyzékkel kapcsolatos eljárások](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures) című témakörben olvashat.

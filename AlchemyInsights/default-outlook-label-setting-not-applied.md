---
title: Nincs Outlook alapértelmezett címkebeállítás
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454753"
---
# <a name="default-outlook-label-setting-not-applied"></a>Nincs Outlook alapértelmezett címkebeállítás

Ha az Outlook alapértelmezett címkebeállítása nem megfelelően van alkalmazva, és egy másik címkét vagy címkét sem alkalmaz, ismert probléma tapasztalható (MC277818), és a probléma megoldásához az alábbi két lehetőség közül valamelyiket kell alkalmaznia:

**1. lehetőség:**

1. A Microsoft 365 Megfelelőségi központ >   >  **információvédelem területén.**
1. Válassza **a Címkeházi** házirendek lehetőséget, és válassza ki a szerkeszteni kívánt címkeházi házirendet ( az **OutlookDefaultlabel** beállítás nincs megfelelően beállítva a szóban forgó címkeházi házirendben. A **beállítás megtekintéséhez futtassa a Get-labelpolicy** beállítást, majd válassza a **Házirend szerkesztése gombra.**
1. Válassza a **Tovább** gombot, amíg meg nem jelenik Az alapértelmezett címke alkalmazása az e-mailekre **beállítás,** amely akkor érhető el, ha bejelöli **A** felhasználók számára kötelező címke alkalmazása az e-mailekre és dokumentumokra címke beállítását a Házirend-beállítások **párbeszédpanelen.**
1. Az Alapértelmezett **címke alkalmazása a** dokumentumokra párbeszédpanelen válassza a **Nincs** lehetőséget a legördülő listából.
1. A **címkebeállítások mentéséhez** **válassza** a Tovább és a Küldés gombot.

**2. lehetőség:**

A [Biztonsági és megfelelőségi központ Powershell-parancsmagjában](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)az Set-LabelPolicy parancsmaggal módosítsa az **OutlookDefaultlabel paramétert** **Nincs** értékre az {OutlookDefaultLabel="None"}.

Futtassa a következőt: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

A feliratok alapértelmezett címkéiről további Outlook A címkék alapértelmezett címkéinek [beállítása Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)
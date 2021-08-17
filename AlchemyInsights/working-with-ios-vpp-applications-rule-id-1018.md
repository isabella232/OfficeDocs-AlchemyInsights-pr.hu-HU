---
title: Az iOS VPP-alkalmazások 1018-as szabályazonosítója
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083016"
---
# <a name="working-with-ios-vpp-applications"></a>Az iOS VPP-alkalmazások alkalmazásai

A mennyiségi vásárlással vásárolt [iOS-appok](https://docs.microsoft.com/intune/vpp-apps-ios) kezelése az Microsoft Intune-et használva további információt az Apple mennyiségi vásárlással kapcsolatos program funkcióiról, korlátairól és a szoftvertámogatás használatának lépéseiről Microsoft Intune.
  
 **Gyakori problémák:** "IOS VPP-appot rendeltem a felhasználóimhoz, de a telepítés nem sikerült."
  
- Ez akkor fordulhat elő, ha több mobileszköz-kezelő szolgáltatónál használ egyetlen VPP-jogkivonatot. Az Apple VPP-jogkivonatai csak egy szolgáltatónál használhatók. Ha több szolgáltatóval használt VPP-jogkivonatot, újra fel kell töltenie a jogkivonatot az Intune-ba.

- A telepítés akkor is meghiúsulhat, ha a telepített telepítések teljes száma meghaladja a licencek számát. A licencek használati jelentésének megtekintéséhez kattintson az **Intune Mobile apps** \> **applicencek lapra.** A licencek használatban való visszaigénylését ebben a cikkben [olvashatja el.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)

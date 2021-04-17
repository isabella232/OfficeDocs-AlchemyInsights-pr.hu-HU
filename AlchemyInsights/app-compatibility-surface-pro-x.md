---
title: Alkalmazáskompatibilitás a Microsoft Surface Pro X-szel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 085815982a3948a7853326541101d2ed21c1869e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837411"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>Alkalmazáskompatibilitás a Microsoft Surface Pro X-szel

Az alkalmazások másképp futnak a Surface Pro X-hez hasonló eszközökön. A legtöbb alkalmazás kompatibilis, vannak azonban bizonyos korlátozások. Az alábbi listában felsoroljuk azokat a problémákat, amelyek az alkalmazások futtatása közben előfordulhatnak: 

**Illesztőprogramok.** Az illesztőprogramok akkor működnek, ha Windows 10-es, ARM pc-n való használatra tervezték. Ha egy illesztőprogram nem működik, az alkalmazás – vagy a hardver, amelyre támaszkodik – sem fog működni. Ha további támogatásra van szükség az eszközéhez, olvassa el a [Windows 10 ARM-alapú PC-k](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5) – gyakori kérdések című témakört, vagy ellenőrizze a hardver gyártóját.

**64 bites (x64-es) alkalmazások.** A 64 bites (x64-es) alkalmazások nem működnek. 64 bites (ARM64-es) alkalmazásokra, 32 bites (ARM32) alkalmazásokra vagy 32 bites (x86-os) alkalmazásokra lesz szüksége. Az appok 32 bites (x86- és 32 bites) verzióját általában megtalálja, egyes alkalmazásfejlesztők azonban csak 64 bites (x64-es) alkalmazásokat kínálnak.

**Testre szabott alkalmazások.** A Windows-élményt testre szabó alkalmazások, például kisegítő technológiák vagy felhőtárhely-alkalmazások problémákat okozhatnak. További információért ellenőrizze az alkalmazás gyártóját.

**Külső víruskereső szoftver.** Egyes külső víruskereső szoftverek nem telepíthetők. A Windows Biztonság révén biztonságban lehet a Windows 10-es eszköze támogatott élettartama alatt.

**Windows Fax és Szkennelés.** A Windows Fax és szkennelés nem érhető el Windows 10 ARM pc-n.

Ha problémákat fog találni egy alkalmazás telepítésével, eltávolításával vagy újratelepítésével kapcsolatban, tekintse át az [Alkalmazás-hibaelhárítás részletei témakört.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)

A ritkán előforduló esetek kivételével az összes kulcsszónak vagy az AND kulcsszónak kell lennie.
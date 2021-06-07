---
title: Az Microsoft Intune biztonsági alapértékek használatával konfigurálhatja Windows 10 eszközöket
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793900"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="e66c0-102">Az Microsoft Intune biztonsági alapértékek használatával konfigurálhatja Windows 10 eszközöket</span><span class="sxs-lookup"><span data-stu-id="e66c0-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="e66c0-103">Az Intune biztonsági alaptervei segítenek megvédeni a felhasználókat és az eszközöket.</span><span class="sxs-lookup"><span data-stu-id="e66c0-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="e66c0-104">A biztonsági alapértékek Windows beállítások, amelyek az adott biztonsági csoportok által ajánlott ismert beállítások és alapértelmezett értékek alkalmazásával előre megadott csoportokra vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="e66c0-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="e66c0-105">Ha létrehoz egy alapterv biztonsági profilt az Intune-ban, olyan sablont hoz létre, amely több eszközkonfigurációs profilból áll.</span><span class="sxs-lookup"><span data-stu-id="e66c0-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="e66c0-106">Amikor biztonsági alapterveket telepít felhasználók vagy eszközök csoportjain vagy eszközein, a beállításokat a rendszer az Windows 10 vagy újabb eszközökön alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="e66c0-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="e66c0-107">A Microsoft mobileszköz-kezelési (MDM) biztonsági alapterve például automatikusan engedélyezi a BitLocker a cserélhető meghajtókon, megköveteli az eszköz zárolásának feloldásához szükséges jelszót, és letiltja az alapvető hitelesítést.</span><span class="sxs-lookup"><span data-stu-id="e66c0-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="e66c0-108">Ha egy alapértelmezett érték nem működik a környezetben, testre szabhatja az alaptervet a szükséges beállítások alkalmazásához.</span><span class="sxs-lookup"><span data-stu-id="e66c0-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="e66c0-109">A biztonsági alapértékek egy végpontok közötti biztonságos munkafolyamatot is Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e66c0-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="e66c0-110">A biztonsági alapértékek a biztonságot befolyásoló beállításokhoz ajánlott eljárásokat és javaslatokat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="e66c0-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="e66c0-111">Intune-partnerek a Windows biztonsági csapatával, amely alapértékeket hoz létre a csoportházirendek számára, így ezek az ajánlások megbízható útmutatáson és kiterjedt tapasztalaton alapulnak.</span><span class="sxs-lookup"><span data-stu-id="e66c0-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="e66c0-112">Ha most először hozza létre az Intune-t, és nem tudja, hol kezdje, a biztonsági alapértékek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt.</span><span class="sxs-lookup"><span data-stu-id="e66c0-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="e66c0-113">Ha jelenleg csoportházirendet használ, a biztonsági alapértékekkel sokkal egyszerűbb az Intune-ra való áttelepítés, mivel ezek az Intune beépített kezelési lehetőségei.</span><span class="sxs-lookup"><span data-stu-id="e66c0-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="e66c0-114">További információt a [](/windows/security/threat-protection/windows-security-baselines) Biztonsági alapértékek Windows mobileszköz-kezelés [– útmutatóban olvashat.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="e66c0-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>


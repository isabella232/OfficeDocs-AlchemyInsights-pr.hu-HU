---
title: A Microsoft Intune biztonsági alaptervek használata a Windows 10-es eszközök beállításához
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694433"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="0efbe-102">A Microsoft Intune biztonsági alaptervek használata Windows 10-es eszközök konfigurálásához</span><span class="sxs-lookup"><span data-stu-id="0efbe-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="0efbe-103">Az Intune biztonsági alaptervei segítenek megvédeni a felhasználókat és az eszközöket.</span><span class="sxs-lookup"><span data-stu-id="0efbe-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="0efbe-104">A biztonsági alapértékek a Windows beállításainak olyan előre konfigurált csoportjai, amelyek a megfelelő biztonsági csoportok által ajánlott ismert beállításokat és alapértelmezett értékcsoportokat alkalmazzák.</span><span class="sxs-lookup"><span data-stu-id="0efbe-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="0efbe-105">Ha létrehoz egy alapbiztonsági profilt az Intune-ban, több eszközkonfigurációs profilból áll egy sablon.</span><span class="sxs-lookup"><span data-stu-id="0efbe-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="0efbe-106">Amikor biztonsági alapértékeket telepít felhasználók vagy eszközök csoportjaira, a beállítások a Windows 10-es vagy újabb verzióin futó eszközökre vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="0efbe-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="0efbe-107">A Microsoft mobileszköz-kezelési (MDM) biztonsági alapterve például automatikusan (1) engedélyezi a BitLocker használatát a cserélhető meghajtókhoz, (2) az eszköz zárolásának feloldásához szükséges jelszót, és (3) letiltja az alapszintű hitelesítést.</span><span class="sxs-lookup"><span data-stu-id="0efbe-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="0efbe-108">Ha egy alapértelmezett érték nem működik a környezetben, testre szabhatja az alaptervet a szükséges beállítások alkalmazásához.</span><span class="sxs-lookup"><span data-stu-id="0efbe-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="0efbe-109">A biztonsági alapértékek szintén segítenek a végpontok közötti biztonságos munkafolyamatok létrehozására a Microsoft 365-ben.</span><span class="sxs-lookup"><span data-stu-id="0efbe-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="0efbe-110">Az alábbiakban a funkció néhány előnyét kínáljuk:</span><span class="sxs-lookup"><span data-stu-id="0efbe-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="0efbe-111">A biztonsági alapértékek a biztonságot befolyásoló beállításokhoz ajánlott eljárásokat és javaslatokat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="0efbe-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="0efbe-112">Mivel az Intune partneri viszonyban van a Windows biztonsági csapatával, amely alapterveket hoz létre a csoportházirendek számára, ezek a javaslatok megbízható útmutatáson és kiterjedt felhasználói élményen alapulnak.</span><span class="sxs-lookup"><span data-stu-id="0efbe-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="0efbe-113">Ha még nem tudja, hogy hol kezdje az Intune-t, akkor a biztonsági alapértékek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt.</span><span class="sxs-lookup"><span data-stu-id="0efbe-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="0efbe-114">Ha jelenleg csoportházirendet használ, akkor a biztonsági alapértékekkel sokkal egyszerűbb az Intune-ra való áttelepítés, mivel ezek a biztonsági alapértékek az Intune beépített funkciói, és a kezelés élvonalbeli funkcióival rendelkeznek.</span><span class="sxs-lookup"><span data-stu-id="0efbe-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="0efbe-115">További információt a Windows biztonsági [alaptervei és](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [a Mobileszköz-kezelés.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="0efbe-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>
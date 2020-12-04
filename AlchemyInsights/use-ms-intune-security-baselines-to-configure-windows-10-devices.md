---
title: Windows 10-es eszközök beállítása a Microsoft Intune biztonsági alaptervek segítségével
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573540"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="00448-102">Windows 10-es eszközök beállítása a Microsoft Intune biztonsági alaptervek segítségével</span><span class="sxs-lookup"><span data-stu-id="00448-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="00448-103">Az Intune biztonsági alaptervek segítenek megvédeni a felhasználókat és az eszközöket.</span><span class="sxs-lookup"><span data-stu-id="00448-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="00448-104">A biztonsági alaptervek a Windows-beállítások előre konfigurált csoportjai, amelyek a beállítások ismert csoportját és a megfelelő biztonsági csoportok által javasolt alapértelmezett értékeket alkalmazzák.</span><span class="sxs-lookup"><span data-stu-id="00448-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="00448-105">Ha az Intune-ban biztonsági alapprofilokat hoz létre, több eszköz-konfigurációs profilból álló sablont hoz létre.</span><span class="sxs-lookup"><span data-stu-id="00448-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="00448-106">Ha a biztonsági alapterveket felhasználók vagy eszközök csoportjaiba telepíti, a beállítások a Windows 10 vagy újabb rendszerű eszközökön érvényesek.</span><span class="sxs-lookup"><span data-stu-id="00448-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="00448-107">Például a MDM biztonsági alapterv automatikusan (1) engedélyezi a BitLocker használatát a cserélhető meghajtókon (2) az eszközök zárolásának feloldásához, és (3) letiltja az egyszerű hitelesítést.</span><span class="sxs-lookup"><span data-stu-id="00448-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="00448-108">Ha egy alapértelmezett érték nem működik a környezetében, az alapterv testreszabásával alkalmazza a szükséges beállításokat.</span><span class="sxs-lookup"><span data-stu-id="00448-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="00448-109">A biztonsági alaptervek a Microsoft 365-ban is segítenek az end-to-end biztonsági munkafolyamatok létrehozásában.</span><span class="sxs-lookup"><span data-stu-id="00448-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="00448-110">Az alábbi előnyök a következők:</span><span class="sxs-lookup"><span data-stu-id="00448-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="00448-111">Egy biztonsági alapterv tartalmazza a biztonsági beállításokat érintő gyakorlati tanácsokat és javaslatokat.</span><span class="sxs-lookup"><span data-stu-id="00448-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="00448-112">Mivel az Intune partnerei a Windows biztonsági csapata alapterveket hoz létre a csoportházirendekhez, ezek az ajánlások a Solid Orientációs és a széleskörű használatot szolgálják.</span><span class="sxs-lookup"><span data-stu-id="00448-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="00448-113">Ha nem biztos abban, hogy hol találja meg az Intune-t, és nem biztos abban, hogy hol találja meg a kezdést, a biztonsági alaptervek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt.</span><span class="sxs-lookup"><span data-stu-id="00448-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="00448-114">Ha jelenleg egy csoportházirendet használ, akkor az Intune felügyeleti célokra való áttelepítése jóval megkönnyíti a biztonsági alaptervek használatát, mivel ezek a felhasználók a Intune szolgáltatásba kerülnek, és magukban foglalják a kezelés élvonalbeli funkcióit.</span><span class="sxs-lookup"><span data-stu-id="00448-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="00448-115">További információt a [Windows biztonsági alaptervek](https://go.microsoft.com/fwlink/?linkid=2141503) és a [mobileszköz-kezelés](https://go.microsoft.com/fwlink/?linkid=2141701)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="00448-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>
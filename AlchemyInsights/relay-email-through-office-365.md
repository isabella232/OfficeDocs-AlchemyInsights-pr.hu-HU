---
title: E-mail-továbbítás az Office 365-ön keresztül
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3c056f5c78935adcf0b64779f9632f9336080a40
ms.sourcegitcommit: dce9cf9bb05d29f0f9bab61fe3fc25e99f0cebf1
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35630743"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="22f91-102">Többfunkciós eszköz vagy alkalmazás beállítása az Office 365-tel való levelezéshez</span><span class="sxs-lookup"><span data-stu-id="22f91-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="22f91-103">A különféle lehetőségekről és az eljárás lépéseiről a [Többfunkciós eszköz vagy alkalmazás beállítása az Office 365-tel való levelezéshez](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4) című cikk nyújt tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="22f91-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="22f91-104">**Megjegyzés:** Ha eszköze vagy alkalmazása rövid ideje nem működik, ne feledje, hogy a közelmúltban a terveknek megfelelően megkezdtük a [3DES titkosítás letiltását](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="22f91-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="22f91-105">Az érintett eszközök megjelenítéséhez nyissa meg az [SMTP-hitelesítést használó ügyfelekről szóló jelentést](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="22f91-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="22f91-106">Gyakori hibák lehetnek a következők: hitelesítési hiba, TLS-hiba, a titkosítási algoritmus hibája, a nem egyező algoritmusok vagy a kapcsolat megszakadása.</span><span class="sxs-lookup"><span data-stu-id="22f91-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="22f91-107">A hiba megoldásához:</span><span class="sxs-lookup"><span data-stu-id="22f91-107">To resolve the issue:</span></span>
 - <span data-ttu-id="22f91-108">**A Windows Server 2003 IIS SMTP a továbbiakban nem fog működni – új Windows-verzió szükséges.**</span><span class="sxs-lookup"><span data-stu-id="22f91-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="22f91-109">Érdeklődjön az alkalmazás vagy az eszköz gyártójánál, hogy van-e lehetőség valamelyik modern titkosítás támogatására, esetleg van-e elérhető frissítés.</span><span class="sxs-lookup"><span data-stu-id="22f91-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>

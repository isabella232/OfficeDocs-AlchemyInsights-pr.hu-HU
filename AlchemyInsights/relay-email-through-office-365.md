---
title: E-mail-továbbítás a Microsoft 365-ön keresztül
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023461"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="1a87b-102">Többfunkciós eszköz vagy alkalmazás beállítása levelek küldéséhez</span><span class="sxs-lookup"><span data-stu-id="1a87b-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="1a87b-103">A különféle lehetőségekről és az eljárás lépéseiről a [Többfunkciós eszköz vagy alkalmazás beállítása a Microsoft 365-tel való levelezéshez](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365) című cikk nyújt tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="1a87b-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="1a87b-104">**Megjegyzés:** Ha eszköze vagy alkalmazása rövid ideje nem működik, ne feledje, hogy a közelmúltban a terveknek megfelelően megkezdtük a [3DES titkosítás letiltását](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="1a87b-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="1a87b-105">Az érintett eszközök megjelenítéséhez nyissa meg az [SMTP-hitelesítést használó ügyfelekről szóló jelentést](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="1a87b-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="1a87b-106">Gyakori hibák lehetnek a következők: hitelesítési hiba, TLS-hiba, a titkosítási algoritmus hibája, a nem egyező algoritmusok vagy a kapcsolat megszakadása.</span><span class="sxs-lookup"><span data-stu-id="1a87b-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="1a87b-107">A hiba megoldásához:</span><span class="sxs-lookup"><span data-stu-id="1a87b-107">To resolve the issue:</span></span>

 - <span data-ttu-id="1a87b-108">**A Windows Server 2003 IIS SMTP a továbbiakban nem fog működni – új Windows-verzió szükséges.**</span><span class="sxs-lookup"><span data-stu-id="1a87b-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="1a87b-109">Érdeklődjön az alkalmazás vagy az eszköz gyártójánál, hogy van-e lehetőség valamelyik modern titkosítás támogatására, esetleg van-e elérhető frissítés.</span><span class="sxs-lookup"><span data-stu-id="1a87b-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>

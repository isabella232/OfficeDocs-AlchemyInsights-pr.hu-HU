---
title: Duplikált eszközrekord a portálon
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814518"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="fa18a-102">Duplikált eszközrekord a portálon</span><span class="sxs-lookup"><span data-stu-id="fa18a-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="fa18a-103">Előfordulhat, hogy a portálon 2 rekord található egy eszközhöz, ha az eszköz nem jelenti megfelelően az együttes felügyeleti állapotát a Konfigurációkezelő webhelynek.</span><span class="sxs-lookup"><span data-stu-id="fa18a-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="fa18a-104">Egy eszköz együttes felügyeleti állapotának ellenőrzéséhez tekintse át az eszközhöz tartozó **Együttes felügyelet** oszlopot a Konfigurációkezelő konzolon.</span><span class="sxs-lookup"><span data-stu-id="fa18a-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="fa18a-105">Ha az oszlop nem látható, akkor a megjelenítéséhez a jobb gombbal bármelyik oszlopfejlécre kattintva kiválaszthatja a listáról.</span><span class="sxs-lookup"><span data-stu-id="fa18a-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="fa18a-106">Az Együttes felügyelet mezőben **Igen** értéknek kell szerepelnie.</span><span class="sxs-lookup"><span data-stu-id="fa18a-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="fa18a-107">Ha az érték **Nem**, nyissa meg a Konfigurációkezelő ügyfélalkalmazást az ügyféleszközön, és ellenőrizze az Általános lapon látható **Együttes felügyelet** tulajdonságot.</span><span class="sxs-lookup"><span data-stu-id="fa18a-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="fa18a-108">Ha a tulajdonság értéke **Engedélyezve**, ez az ügyfél és a felügyeleti pont közötti kommunikációval kapcsolatos problémákra utal.</span><span class="sxs-lookup"><span data-stu-id="fa18a-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="fa18a-109">Tekintse át a **CcmMessaging.log** fájlt az eszközön a lehetséges kapcsolódási hibák kivizsgálásához.</span><span class="sxs-lookup"><span data-stu-id="fa18a-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="fa18a-110">Ha az érték **Letiltva**, és az eszköz regisztrálva van az Intune szolgáltatásban, akkor győződjön meg arról, hogy az eszköz megkapta az együttes felügyeleti házirendet; ehhez tekintse át a **CoManagementHandler.log** fájlt az eszközön.</span><span class="sxs-lookup"><span data-stu-id="fa18a-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>

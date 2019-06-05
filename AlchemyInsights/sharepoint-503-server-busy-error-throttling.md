---
title: A SharePoint Online szabályozása
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716929"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="46cec-102">A SharePoint Online szabályozása</span><span class="sxs-lookup"><span data-stu-id="46cec-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="46cec-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Jelenhet meg egy 503 kiszolgáló foglalt hiba, menjen el a OneDrive vagy a Sharepoint-webhelyek tett kísérlet közben.</span></span><span class="sxs-lookup"><span data-stu-id="46cec-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="46cec-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ezt a hibát okozhatja a Sharepoint szolgáltatáson belül szabályozását. A SharePoint Online használ szabályozását az optimális teljesítmény és a SharePoint Online szolgáltatás megbízhatóságának fenntartására. Szabályozási határértékek a száma, a felhasználói műveletek vagy egyidejű hívások (parancsfájl vagy kód) által erőforrások túlfelhasználást megakadályozása érdekében. Ha Ön kap folyamatban, 99 %-ában egyéni kód miatt van.</span></span><span class="sxs-lookup"><span data-stu-id="46cec-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="46cec-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">További információt lásd, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">ne beolvasása folyamatban, vagy blokkolja a SharePoint Online</a>-szabályozás.</span></span><span class="sxs-lookup"><span data-stu-id="46cec-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="46cec-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ha úgy gondolja, hogy ez a hiba akkor független a sávszélesség-szabályozás, ha nincs aktív karbantartási <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>navigáljon a bérlő bekövetkező ellenőrizheti. Végezetül ellenőrizze, akkor látogassa meg a <a href="https://portal.office.com/adminportal/home#/servicehealth">Egészségügyi szolgáltatás</a> , amely felmerülhet tanácsadók/események ellenőrzése.</span></span><span class="sxs-lookup"><span data-stu-id="46cec-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>



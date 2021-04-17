---
title: Az EWS szabályozási beállításainak módosítása
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818038"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="5fa9e-102">Az EWS szabályozási beállításainak módosítása</span><span class="sxs-lookup"><span data-stu-id="5fa9e-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="5fa9e-103">Kérjük, futtassa automatizált tesztünket, amely lehetővé teszi az EWS-szabályozási házirend módosítását az áttelepítés ideje alatt.</span><span class="sxs-lookup"><span data-stu-id="5fa9e-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="5fa9e-104">Vegye figyelembe, hogy az EWS-importok postaládánként 5 percenként 150 MB-ra korlátozva maradnak a futtatás után is; ha nagyobb átviteli sebességet szeretne elérni, kérjük, telepítsen át egyszerre több felhasználót.</span><span class="sxs-lookup"><span data-stu-id="5fa9e-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="5fa9e-105">Felhívjuk a figyelmét arra, hogy az EWS-szabályozási házirendek módosítása nincs hatással a következő áttelepítési típusokra (a Microsoft eszközeinek használatával): hibrid, átállásos/szakaszos (RPC/HTTP), IMAP, G Suite, nyilvános mappa vagy PST-importálási szolgáltatás.</span><span class="sxs-lookup"><span data-stu-id="5fa9e-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>
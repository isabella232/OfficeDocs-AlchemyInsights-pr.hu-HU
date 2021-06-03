---
title: A endpoint DLP not deployed to user's device
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731586"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>A endpoint DLP not deployed to user's device

Ha a Végpontok adatveszteség-megelőzés (DLP) beállítás nem vonatkozik egy felhasználó eszközére, ellenőrizze, hogy megfelel-e az alábbi követelményeknek:

- Windows 10 x64-es build 1809-es vagy újabb build telepítve van az eszközön.
- A kártevők elleni ügyfélprogram 4.18.2009.7-es vagy újabb verziója telepítve van.
- Az eszköz **az alábbi** eszközök egyike:
    
    - Azure Active Directory (Azure AD) csatlakozva
    - Hibrid Azure AD-csatlakozás
    - AAD regisztrálva

- A házirendműveletek érvénybe lépésekhez győződjön meg arról, Chromium microsoft Chromium Edge böngésző telepítve van a végponteszközre.

Az Endpoint DLP üzembe helyezésének további követelményeiről az Első lépések [az végpontok adatveszteség-megelőzési szolgáltatásával .](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)
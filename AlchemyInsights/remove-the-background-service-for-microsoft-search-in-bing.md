---
title: A Microsoft Search háttérszolgáltatásának eltávolítása a Bingben
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816201"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>A Microsoft Search háttérszolgáltatásának eltávolítása a Bingben

Ha el szeretné távolítani a Microsoft Search háttérszolgáltatását a Bingben, próbálkozzon az alábbi megoldásokkal:

1. Az eredeti keresőmotor-beállításokhoz való visszatéréshez tegye a következőket:

    a. Kapcsolja ki a Bing használata alapértelmezett keresőmotorként **kapcsolót. [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**

    b. [A Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) Felügyeleti központban törölje a szervezet minden felhasználóját érintő beállítást.

2. Ha el szeretné távolítani a háttérszolgáltatást egy adott eszközről, tegye a következőket:

    a. Válassza **a Vezérlőpult > Programok > szolgáltatások lehetőséget.**

    b. Kattintson a jobb **gombbal a Microsoft Search elemre** a Bingben a telepített programok listája alatt, és kattintson az Eltávolítás **parancsra.**

3. Ha a háttérszolgáltatást több eszközről szeretné eltávolítani a szervezetből, jelentkezzen be rendszergazdaként, és futtassa az alábbi parancsot egy parancsfájlban: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`

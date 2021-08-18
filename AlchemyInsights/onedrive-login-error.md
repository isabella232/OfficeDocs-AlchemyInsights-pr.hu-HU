---
title: OneDrive bejelentkezési hiba az AADSTS50011-ben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112914"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive bejelentkezési hiba az AADSTS50011-ben

Ha "AADSTS50011: A kérelemben megadott válasz URL-címe nem egyezik meg a válasz" hibaüzenet jelenik meg az OneDrive appba való bejelentkezéskor, ellenőrizze az alábbiakat:

A OneDrive verziónak a 20.052.XXXX.XXXX. verziónál nem kisebbnek kell lennie. A verzió ellenőrzéshez kattintson a kék OneDrive ikonra az értesítési területen, és válassza **a Súgó & Gépház > Gépház > About lehetőséget.**

Előfordulhat, hogy a hálózata blokkolja a g.live.com **és** a **oneclient.sfx.ms.** Ha a forgalom le van tiltva, a OneDrive nem tudja frissíteni magát. A hálózati rendszergazdával működve győződjön meg arról, hogy rendelkezik hozzáféréssel az ilyen URL-címekhez. [Ezeknek a végpontoknak](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) elérhetőnek kell lennie a Microsoft 365 használó ügyfelek számára.

Ha manuálisan kell lekérte a verziók aktuális OneDrive, látogasson el [https://aka.ms/getonedrive](https://aka.ms/getonedrive) a webhelyre.

---
title: A Microsoft 365 Felügyeleti központ jelentéseiben nem olvasható a felhasználónév
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327816"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>A Microsoft 365 Felügyeleti központ jelentéseiben nem olvasható a felhasználónév

A Microsoft 365 Felügyeleti központ jelentései nem jelenítik meg a felhasználóneveket, hanem alfanumerikus értékek olvashatók, például B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ez elvárt viselkedés és az Üzenetközpontban (MC275344, 2021. augusztus 3-án közzétéve) jelent meg. 

A globális rendszergazdák visszaállíthatják ezt a változást a bérlői fiókjukra, és ha a szervezet adatvédelmi gyakorlata lehetővé teszi, személyek azonosítására alkalmas felhasználói adatokat is tartalmazhatnak. A módosítás visszaállításához a bérlő számára:

1. A Felügyeleti központban válassza a **Beállítások**  >  **Szervezeti beállítások**  >  [**Szolgáltatások**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )lehetőséget, majd válassza a **Jelentések** lehetőséget. 
1. A **Felhasználói adatok megjelenítési módjának kiválasztása** alatt válassza az **Azonosítható felhasználói adatok megjelenítése a jelentésekben** lehetőséget, majd futtassa újra a jelentést.
---
title: A jelentésekben Microsoft 365 Felügyeleti központ nem olvasható felhasználónév
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
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316200"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>A jelentésekben Microsoft 365 Felügyeleti központ nem olvasható felhasználónév

A Microsoft 365 Felügyeleti központ jelentések nem jelenítik meg a felhasználóneveket, hanem alfanumerikus értékeket, például B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ez a viselkedés elvárt , és az Üzenetközpontban (MC275344, 2021. augusztus 3-án közzétéve) jelent meg. 

A globális rendszergazdák visszaállíthatják ezt a változást a bérlői fiókjukra, és ha a szervezet adatvédelmi gyakorlata lehetővé teszi, személyek azonosítására alkalmas felhasználói adatokat is tartalmaznak. A módosítás visszaváltása a bérlőhöz:

1. A felügyeleti központban válassza a **Szervezeti Gépház**  >  **szolgáltatások**  >  [](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)gombra, és válassza a Jelentések **lehetőséget.** 
1. A **Felhasználói adatok megjelenítése csoportban** válassza az Azonosítható **felhasználói** adatok megjelenítése a jelentésekben lehetőséget, majd futtassa újra a jelentést.
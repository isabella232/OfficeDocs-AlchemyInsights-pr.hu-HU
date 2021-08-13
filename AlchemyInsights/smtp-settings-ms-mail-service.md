---
title: A levelezési szolgáltatás SMTP Microsoft 365 beállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813973"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>A levelezési szolgáltatás SMTP Microsoft 365 beállítása

A levelezési szolgáltatások SMTP-beállításai az alábbi Microsoft 365:

**Kiszolgáló:** smtp.office365.com </br>
**Port:** 587 </br>
**Titkosítás:** STARTTLS (csak a TLS 1.2-es verzió támogatott. Ellenőrizze, hogy az alkalmazás vagy eszköz támogatja-e a TLS 1.2-es adatokat) </br>
**Felhasználónév:** Az Ön Office 365 címe (például example@yourdomain.com) </br>
**Jelszó:** A Office 365 jelszava </br>
**Hitelesítés:** Kötelező </br>
**Küldési korlátok:** 10 000 e-mail naponta </br>

A POP- és IMAP-beállításokról a [POP-, IMAP- és SMTP-beállítások.](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)
 
Az e-mailek Microsoft 365-fiókkal való továbbítására vonatkozó lehetőségekről és a lépésekről a Többfunkciós eszköz vagy alkalmazás beállítása e-mail-küldésre a Microsoft 365 vagy az [Office 365.](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)
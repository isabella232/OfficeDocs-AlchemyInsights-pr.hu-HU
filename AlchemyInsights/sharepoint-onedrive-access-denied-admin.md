---
title: A hozzáférés megtagadva üzenetet – problémamegoldás
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716649"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Üzenetek megtagadta a hozzáférést a Sharepoint/OneDrive Admin Center – problémamegoldás

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Ha a hozzáférés megtagadásáról, tallózással keresse meg a Sharepoint/OneDrive Admin Center megkísérelte kap, győződjön meg arról, hogy <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">a felhasználó licenc hozzárendelése </a>. Ha a felhasználói licenccel rendelkezik, akkor győződjön meg arról is <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">egy rendszergazda szerepkört</a> , amelyhez hozzáférhet az admin-centers.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Ez a probléma akkor is előfordulhat, amikor a felhasználó törli, és újra létrehozza a ugyanolyan egyszerű felhasználónév (UPN). Az új fiók jön létre egy másik értéket PUID (Passport egyedi azonosító) segítségével. Ha a felhasználó megpróbál hozzáférni egy webhelycsoport vagy a OneDrive, a felhasználó rendelkezik egy helytelen PUID. A második forgatókönyv magában foglalja a könyvtár szinkronizálás az Active Directory szervezeti egységet (OU). Ha a felhasználó rendelkezik már bejelentkezett a SharePoint, majd átkerül egy másik szervezeti egység és SharePoint resynced, akkor ez a probléma tapasztalhatnak.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">A probléma megoldásához a cikk <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">az Office 365 rendszerben a felhasználó visszaállítási</a>lépéseket az eredeti UPN kell visszaállítani.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Megjegyzés:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">a OneDrive vagy a SharePoint felügyeleti központ több felhasználó, aki korábban a hozzáférés nem érhető el, ha az a szolgáltatás átmeneti probléma lehet.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Ellenőrzése a szolgáltatás egészségügyi irányítópult</span></a>.</span></em></span></span></p>



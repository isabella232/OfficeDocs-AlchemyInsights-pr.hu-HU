---
title: Csoport hozzáadása egy SharePoint-webhely
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719484"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>A SharePoint Online kapcsolattal rendelkező hely csoport létrehozása

<p><strong>Van néhány általános problémát észlelt létrehozása, vagy hozza létre újra a csoport webhely kapcsolat.&nbsp;</strong></p>  <p>1.Ha törölt egy csoport és a kapcsolódó webhely, és létrehoz egy másik webhely ugyanazt az URL-címmel, szüksége lesz a végleges eltávolítása az előző webhelyhez.</p>  <ul>  <li>Letöltés <a title="Sao felügyeleti rendszerhéj" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Sao felügyeleti rendszerhéj</a> - kapcsolatban további információ a Bevezetés a powershell, <a title="Bevezetés a SharePoint Online felügyeleti rendszerhéj" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Bevezetés a SharePoint Online felügyeleti rendszerhéj</a>. <br /><br /></li>  <li>Törölt webhelyek használatával a webhely eltávolítása a <a title="eltávolítása-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Eltávolítás-SPODeletedSite</a> powershell parancsmag.</li>  </ul>  <p>Ha egy csoport kapcsolódó webhely létrehozása, és figyelmeztetést küld <strong>egy másik csoportot ugyanazzal az aliasnévvel már létezik</strong>, ellenőrizze a meglévő csoportok a <a title="Office 365 felügyeleti Center" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Az Office 365 felügyeleti Center</a>. A probléma megoldásához, törli a meglévő csoportot, ha már nincs szüksége, vagy hozzon létre egy másikat a webhely kap.&nbsp;</p>  <p><strong>Különböző módon lehet létrehozni és modern csoportok használata a SharePoint.&nbsp;</strong></p>  <ol>  <li>Az Office 365 csoport meglévő webhelyekhez csatlakozhat. További információért lásd: <a title="az Office 365 csoport segítségével a SharePoint felhasználói ineterface csatlakozás" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Csatlakozás az Office 365 csoport segítségével a SharePoint felhasználói ineterface</a>.</li>  <li>Az Office 365 csoport kapcsolattal rendelkező hely létrehozásához szüksége lesz a csoportwebhely létrehozása. További információért lásd: <a title="a SharePoint csoportwebhelyet létrehozása" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Hozzon létre a SharePoint csoportwebhelyet.</a></li>  </ol>


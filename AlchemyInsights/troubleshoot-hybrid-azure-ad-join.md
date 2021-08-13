---
title: Hybrid Azure AD csatlakozás
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939273"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Hybrid Azure AD csatlakozás

Erősen ajánlott annak biztosítása, hogy egy eszköz hozzáférjen a rendszerfiókban található eszköz-regisztráció végpontjaihoz az [eszköz-regisztráció csatlakozási parancsprogramjának](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) használatával.

1. Ha első alkalommal hoz létre eszközregisztrációkat, tekintse át a [Bevezetés az Azure Active Directory eszközkezelésbe](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) témakört, és megtudhatja, hogy miként irányíthatja az eszközöket az Azure AD ellenőrzése alatt.
1. Ha közvetlenül regisztrál eszközöket az Azure AD-be, és feliratkozik velük az Intune-ba, akkor győződjön meg arról, hogy [konfigurálta az Intune-t](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support), és elsőként a [licencelést](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) jelölte meg.
1. Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban és a helyszíni AD-ban. Az eszközregisztrációk beállításait csak az Azure AD globális rendszergazdája kezelheti. Ezenkívül ha automatikus regisztrációt hoz létre a helyszíni Active Directoryban, akkor az Active Directory és az Active Directory FS (ha van) rendszergazdájának kell lennie.

A hibrid illesztés esetleges problémáinak megoldásáról lásd [A hibrid csatlakozás hibaelhárítása](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) témakört a hibrid Azure AD-eszközökhöz való csatlakozásról, valamint az eszközkezelés az Azure AD portálon keresztüli beállításáról lásd [Az Azure AD-hez csatlakozott hibrid eszközök beállítása](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) és az [Eszközök kezelése az Azure portal használatával](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support) témaköröket.

A hibrid Azure Active Directory csatlakozás gyakori problémáinak megoldásáról lásd: [Az Azure AD-hez való hibrid csatlakozás - gyakori kérdések](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).

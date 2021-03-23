---
title: Service Connection Point (SCP) konfigurálása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036143"
---
# <a name="configure-service-connection-point-scp"></a>Service connection Point (SCP) konfigurálása

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Ok:** Nem lehet olvasni az SCP-objektumot és beolvasni az Azure AD bérlői adatait
- **Megoldás:** Tanulmányozza a Szolgáltatás csatlakozási [pont beállítása című szakaszt.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Akcióterv**

- Ellenőrizze, hogy az eszköz megkapta-e a GPO-t a szabályozott ellenőrzéshez.
- Győződjön meg arról, hogy a beállításjegyzék-objektum létrehozta a beállításkulcsokat.
- Győződjön meg arról, hogy a címtárazonosítóhoz és az onmicrosoft tartományhoz két kulcs van létrehozva.

**Az ügyféloldali beállításjegyzék SCP-beállításának konfigurálása**

Az alábbi példában egy csoportházirend-objektumot létrehozva egy olyan beállításjegyzék-beállítást telepíthet, amely konfigurál egy SCP-bejegyzést az eszközök beállításjegyzékében.

1. Nyisson meg egy Csoportházirend kezelése konzolt, és hozzon létre egy új csoportházirend-objektumot a tartományában.
     - Nevezze el az újonnan létrehozott GPO-t (például ClientSideSCP).

2. Szerkessze a GPO-t, és keresse meg a következő elérési utat: Számítógép konfigurációja **> Beállítások > Windows beállítások > beállításjegyzékben.**

3. Kattintson a jobb gombbal a **Beállításjegyzék elemre,** és válassza az > **beállításjegyzék-elem lehetőséget.**

4. Az Általános **lapon** adja meg az alábbiakat:
  
- **Művelet:** Frissítés
    
- **Hive:** HKEY_LOCAL_MACHINE
    
- **Kulcs elérési útja:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Érték neve:** TenantId
    
- **Érték típusa:** REG_SZ
    
- **Értékadatok:** Az Azure AD-példány GUID vagy címtárazonosítója (ez az érték megtalálható az Azure Portal > Azure Active Directory > Tulajdonságai > **Címtárazonosító**)
 
- Kattintson az **OK** gombra.
 
5. Kattintson a jobb gombbal a **Beállításjegyzék elemre,** és válassza az > **beállításjegyzék-elem lehetőséget.**

6. Az Általános **lapon** adja meg az alábbiakat:
  
- **Művelet:** Frissítés
    
- **Hive:** HKEY_LOCAL_MACHINE
    
- **Kulcs elérési útja:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Érték neve:** TenantName
    
- **Érték típusa:** REG_SZ
    
- **Értékadatok:** Az igazolt tartománynév, ha összevont környezetet használ (például AD FS). Az igazolt tartományneve vagy onmicrosoft.com tartományneve (például: contoso.onmicrosoft).com felügyelt környezetben

- Kattintson az **OK** gombra.

7. Zárja be az újonnan létrehozott objektum-objektum szerkesztőjét.

8. Csatolja az újonnan létrehozott GPO-t a kívánt szervezeti egységhez, amely a szabályozott bevezetési sokasághoz tartozó, tartományhoz csatlakozott számítógépeket tartalmazza.

További információ: A hibrid Azure AD-csatlakozás ellenőrzött érvényesítése [– Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs .](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)










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
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="47989-102">Service connection Point (SCP) konfigurálása</span><span class="sxs-lookup"><span data-stu-id="47989-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="47989-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="47989-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="47989-104">**Ok:** Nem lehet olvasni az SCP-objektumot és beolvasni az Azure AD bérlői adatait</span><span class="sxs-lookup"><span data-stu-id="47989-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="47989-105">**Megoldás:** Tanulmányozza a Szolgáltatás csatlakozási [pont beállítása című szakaszt.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="47989-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="47989-106">**Akcióterv**</span><span class="sxs-lookup"><span data-stu-id="47989-106">**Action plan**</span></span>

- <span data-ttu-id="47989-107">Ellenőrizze, hogy az eszköz megkapta-e a GPO-t a szabályozott ellenőrzéshez.</span><span class="sxs-lookup"><span data-stu-id="47989-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="47989-108">Győződjön meg arról, hogy a beállításjegyzék-objektum létrehozta a beállításkulcsokat.</span><span class="sxs-lookup"><span data-stu-id="47989-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="47989-109">Győződjön meg arról, hogy a címtárazonosítóhoz és az onmicrosoft tartományhoz két kulcs van létrehozva.</span><span class="sxs-lookup"><span data-stu-id="47989-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="47989-110">**Az ügyféloldali beállításjegyzék SCP-beállításának konfigurálása**</span><span class="sxs-lookup"><span data-stu-id="47989-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="47989-111">Az alábbi példában egy csoportházirend-objektumot létrehozva egy olyan beállításjegyzék-beállítást telepíthet, amely konfigurál egy SCP-bejegyzést az eszközök beállításjegyzékében.</span><span class="sxs-lookup"><span data-stu-id="47989-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="47989-112">Nyisson meg egy Csoportházirend kezelése konzolt, és hozzon létre egy új csoportházirend-objektumot a tartományában.</span><span class="sxs-lookup"><span data-stu-id="47989-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="47989-113">Nevezze el az újonnan létrehozott GPO-t (például ClientSideSCP).</span><span class="sxs-lookup"><span data-stu-id="47989-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="47989-114">Szerkessze a GPO-t, és keresse meg a következő elérési utat: Számítógép konfigurációja **> Beállítások > Windows beállítások > beállításjegyzékben.**</span><span class="sxs-lookup"><span data-stu-id="47989-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="47989-115">Kattintson a jobb gombbal a **Beállításjegyzék elemre,** és válassza az > **beállításjegyzék-elem lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="47989-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="47989-116">Az Általános **lapon** adja meg az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="47989-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="47989-117">**Művelet:** Frissítés</span><span class="sxs-lookup"><span data-stu-id="47989-117">**Action**: Update</span></span>
    
- <span data-ttu-id="47989-118">**Hive:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="47989-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="47989-119">**Kulcs elérési útja:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="47989-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="47989-120">**Érték neve:** TenantId</span><span class="sxs-lookup"><span data-stu-id="47989-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="47989-121">**Érték típusa:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="47989-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="47989-122">**Értékadatok:** Az Azure AD-példány GUID vagy címtárazonosítója (ez az érték megtalálható az Azure Portal > Azure Active Directory > Tulajdonságai > **Címtárazonosító**)</span><span class="sxs-lookup"><span data-stu-id="47989-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="47989-123">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="47989-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="47989-124">Kattintson a jobb gombbal a **Beállításjegyzék elemre,** és válassza az > **beállításjegyzék-elem lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="47989-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="47989-125">Az Általános **lapon** adja meg az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="47989-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="47989-126">**Művelet:** Frissítés</span><span class="sxs-lookup"><span data-stu-id="47989-126">**Action**: Update</span></span>
    
- <span data-ttu-id="47989-127">**Hive:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="47989-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="47989-128">**Kulcs elérési útja:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="47989-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="47989-129">**Érték neve:** TenantName</span><span class="sxs-lookup"><span data-stu-id="47989-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="47989-130">**Érték típusa:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="47989-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="47989-131">**Értékadatok:** Az igazolt tartománynév, ha összevont környezetet használ (például AD FS).</span><span class="sxs-lookup"><span data-stu-id="47989-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="47989-132">Az igazolt tartományneve vagy onmicrosoft.com tartományneve (például: contoso.onmicrosoft).com felügyelt környezetben</span><span class="sxs-lookup"><span data-stu-id="47989-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="47989-133">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="47989-133">Click **OK**.</span></span>

7. <span data-ttu-id="47989-134">Zárja be az újonnan létrehozott objektum-objektum szerkesztőjét.</span><span class="sxs-lookup"><span data-stu-id="47989-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="47989-135">Csatolja az újonnan létrehozott GPO-t a kívánt szervezeti egységhez, amely a szabályozott bevezetési sokasághoz tartozó, tartományhoz csatlakozott számítógépeket tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="47989-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="47989-136">További információ: A hibrid Azure AD-csatlakozás ellenőrzött érvényesítése [– Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs .](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)</span><span class="sxs-lookup"><span data-stu-id="47989-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>










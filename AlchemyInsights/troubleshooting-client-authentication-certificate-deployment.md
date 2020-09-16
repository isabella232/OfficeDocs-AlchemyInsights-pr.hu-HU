---
title: Ügyfél-hitelesítési tanúsítvány telepítésének hibaelhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658988"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="36ae5-102">Ügyfél-hitelesítési tanúsítvány telepítésének hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="36ae5-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="36ae5-103">Az Intune NDES/SCEP és a PKCS/PFX-ügyfél tanúsítványok profiljait gyakran használják más profilokhoz, például a WiFi-hez, a VPN-hez és a levelezéshez, hogy a felhasználók a vállalati forrásokban legyenek hitelesítve.</span><span class="sxs-lookup"><span data-stu-id="36ae5-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="36ae5-104">Ha ezek a profilok az ügyfél tanúsítvány-profiljához kapcsolódnak, attól függ, hogy milyen sikeres volt a profil bevezetése.</span><span class="sxs-lookup"><span data-stu-id="36ae5-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="36ae5-105">A kezdeti infrastruktúra-beállítás és az ügyfél tanúsítvány-profiljának társított konfigurációja gyakran hibaelhárítást igényel.</span><span class="sxs-lookup"><span data-stu-id="36ae5-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="36ae5-106">A NDES-összekötők sikeres beállításának lépésenkénti útmutatója és a tanúsítványok telepítésével kapcsolatos hibaelhárítási útmutató a következő témakörökben található:</span><span class="sxs-lookup"><span data-stu-id="36ae5-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="36ae5-107">Infrastruktúra beállítása az Intune-SCEP támogatásához</span><span class="sxs-lookup"><span data-stu-id="36ae5-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="36ae5-108">A SCEP hibaelhárítása a Microsoft Intune szolgáltatással – áttekintés</span><span class="sxs-lookup"><span data-stu-id="36ae5-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="36ae5-109">A hivatkozott PowerShell-parancsfájlok segítségével ellenőrizheti a konfigurációt.</span><span class="sxs-lookup"><span data-stu-id="36ae5-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="36ae5-110">További információt az [Intune tanúsítvány-összekötő ellenőrző parancsfájljai](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="36ae5-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="36ae5-111">**Egyéb gyakori problémák**</span><span class="sxs-lookup"><span data-stu-id="36ae5-111">**Other common issues**</span></span>

<span data-ttu-id="36ae5-112">**Amikor megpróbálom telepíteni az Intune-tanúsítvány összekötőt az NDES összekötő kiszolgálójára, a következő hibaüzenet jelenik meg: "a tanúsítvány kérésének jelszava nem ellenőrizhető. Lehet, hogy már használta. Új jelszó beolvasása a kéréssel való elküldés céljából**</span><span class="sxs-lookup"><span data-stu-id="36ae5-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="36ae5-113">Ez az üzenet azt jelzi, hogy rendszergazdaként kell futtatnia a tanúsítvány-összekötőt.</span><span class="sxs-lookup"><span data-stu-id="36ae5-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="36ae5-114">Bizonyos környezetekben azok a kiszolgálók, amelyekben az Intune-tanúsítvány fut, proxykiszolgálót kell használniuk ahhoz, hogy csatlakozhasson az Intune-hoz, és így a bizonyítvány-összekötőnek proxyt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="36ae5-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="36ae5-115">Bizonyos körülmények között a NDES összekötő figyelmen kívül hagyja a konfigurált proxybeállításokat, ezért szükség lehet a proxybeállítások konfigurálására a LocalSystem biztonsági környezetében.</span><span class="sxs-lookup"><span data-stu-id="36ae5-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="36ae5-116">A megoldás az, ha az Internet Explorer rendszert futtatja, és egy proxyt konfigurál az IE-ben.</span><span class="sxs-lookup"><span data-stu-id="36ae5-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="36ae5-117">A Intune-összekötő szolgáltatás újraindítása után a NDES összekötő az Intune szolgáltatáshoz csatlakozik.</span><span class="sxs-lookup"><span data-stu-id="36ae5-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="36ae5-118">**A felhasználói eszközök ezentúl nem kapják meg a SCEP-tanúsítványokat a NDES.**</span><span class="sxs-lookup"><span data-stu-id="36ae5-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="36ae5-119">Előfordulhat, hogy az NDES-kiszolgálónak kiállított ügyfél-hitelesítési tanúsítvány, amelyet az NDES összekötő telepítése során megadott, lejárt vagy hiányzik.</span><span class="sxs-lookup"><span data-stu-id="36ae5-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="36ae5-120">Megoldás:</span><span class="sxs-lookup"><span data-stu-id="36ae5-120">To resolve:</span></span> 
 
1. <span data-ttu-id="36ae5-121">Távolítsa el a NDES összekötőt.</span><span class="sxs-lookup"><span data-stu-id="36ae5-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="36ae5-122">Az alábbi adatok segítségével igényelhet új ügyfél-vagy kiszolgálói hitelesítési tanúsítványt:</span><span class="sxs-lookup"><span data-stu-id="36ae5-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="36ae5-123">Tárgy neve: CN = külső FQDN</span><span class="sxs-lookup"><span data-stu-id="36ae5-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="36ae5-124">Alárendelt alternatív név (mindkettő szükséges): DNS = külső FQDN, DNS = belső FQDN</span><span class="sxs-lookup"><span data-stu-id="36ae5-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="36ae5-125">Telepítse újra az NDES-összekötőt az új tanúsítvánnyal.</span><span class="sxs-lookup"><span data-stu-id="36ae5-125">Reinstall the NDES connector with the new certificate.</span></span>
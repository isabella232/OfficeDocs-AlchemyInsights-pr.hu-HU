---
title: Ügyfélhitelesítési tanúsítványok telepítésének hibaelhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555308"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="10b3b-102">Ügyfélhitelesítési tanúsítványok telepítésének hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="10b3b-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="10b3b-103">Az Intune NDES/SCEP és PKCS/PFX ügyféltanúsítvány-profilokat általában más profiltípusokkal, például a Wifivel, a VPN-nel és az e-mailekkel együtt használják, hogy a felhasználók hitelesíthessék magukat a vállalati erőforrásokban.</span><span class="sxs-lookup"><span data-stu-id="10b3b-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="10b3b-104">Ha ezek a profiltípusok egy ügyféltanúsítvány-profilhoz vannak csatolva, az adott profil sikeres üzembe helyezésétől függ.</span><span class="sxs-lookup"><span data-stu-id="10b3b-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="10b3b-105">Az infrastruktúra kezdeti beállítása és az ügyféltanúsítvány-profil kapcsolódó konfigurációja gyakran hibaelhárítást igényel.</span><span class="sxs-lookup"><span data-stu-id="10b3b-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="10b3b-106">Az NDES-összekötő sikeres beállításának lépésről lépésre történő útmutatóját és a tanúsítványtelepítéssel kapcsolatos problémák elkülönítésére vonatkozó hibaelhárítási útmutatást a következő témakörökben talál:</span><span class="sxs-lookup"><span data-stu-id="10b3b-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="10b3b-107">Infrastruktúra konfigurálása az SCEP és az Intune támogatásához</span><span class="sxs-lookup"><span data-stu-id="10b3b-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="10b3b-108">Az SCEP-tanúsítványprofilok Microsoft Intune-nal való hibaelhárításának áttekintése</span><span class="sxs-lookup"><span data-stu-id="10b3b-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="10b3b-109">A hivatkozott powershell-parancsfájlok segítségével ellenőrizze a konfigurációt.</span><span class="sxs-lookup"><span data-stu-id="10b3b-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="10b3b-110">További információ: [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="10b3b-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="10b3b-111">**Egyéb gyakori problémák**</span><span class="sxs-lookup"><span data-stu-id="10b3b-111">**Other common issues**</span></span>

<span data-ttu-id="10b3b-112">**Amikor megpróbálom telepíteni az Intune tanúsítványösszekötőt az NDES-összekötő kiszolgálóra, a következő üzenet jelenik meg: "A tanúsítványkérelemben szereplő jelszó nem ellenőrizhető. Lehet, hogy már használták. Szerezzen be egy új jelszót, amelyet ezzel a kéréssel kell beküldenie."**</span><span class="sxs-lookup"><span data-stu-id="10b3b-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="10b3b-113">Ez az üzenet azt jelenti, hogy rendszergazdaként kell futtatnia a tanúsítványösszekötő telepítését.</span><span class="sxs-lookup"><span data-stu-id="10b3b-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="10b3b-114">Bizonyos környezetekben az Intune-tanúsítványt használó kiszolgálóknak proxykiszolgálót kell használniuk az Intune-hoz való csatlakozáshoz, ezért a tanúsítvány-összekötőnek proxyt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="10b3b-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="10b3b-115">Bizonyos körülmények között az NDES-összekötő figyelmen kívül hagyja a konfigurált proxybeállításokat, és szükség lehet a proxybeállítások konfigurálására a LocalSystem biztonsági környezetében való futtatás közben.</span><span class="sxs-lookup"><span data-stu-id="10b3b-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="10b3b-116">A megoldás az, hogy futtassa az Internet Explorer rendszer, és konfigurálja a proxy IE.</span><span class="sxs-lookup"><span data-stu-id="10b3b-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="10b3b-117">Az Intune Connector szolgáltatás újraindítása után az NDES-összekötő csatlakozik az Intune-hoz.</span><span class="sxs-lookup"><span data-stu-id="10b3b-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="10b3b-118">**A felhasználói eszközök már nem kapnak SCEP-tanúsítványokat az NDES-től.**</span><span class="sxs-lookup"><span data-stu-id="10b3b-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="10b3b-119">Lehetséges, hogy az NDES-kiszolgáló számára kiállított és az NDES-összekötő telepítése során megadott ügyfélhitelesítési tanúsítvány lejárt vagy hiányzik.</span><span class="sxs-lookup"><span data-stu-id="10b3b-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="10b3b-120">A probléma megoldása:</span><span class="sxs-lookup"><span data-stu-id="10b3b-120">To resolve:</span></span> 
 
1. <span data-ttu-id="10b3b-121">Távolítsa el az NDES-összekötőt.</span><span class="sxs-lookup"><span data-stu-id="10b3b-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="10b3b-122">Az alábbi adatok kal új ügyfélhitelesítési vagy kiszolgálói hitelesítési tanúsítványt kérhet:</span><span class="sxs-lookup"><span data-stu-id="10b3b-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="10b3b-123">Tulajdonos neve: CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="10b3b-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="10b3b-124">Tulajdonos alternatív neve (mindkettő kötelező): DNS=external fqdn, DNS=internal fqdn</span><span class="sxs-lookup"><span data-stu-id="10b3b-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="10b3b-125">Telepítse újra az NDES-összekötőt az új tanúsítvánnyal.</span><span class="sxs-lookup"><span data-stu-id="10b3b-125">Reinstall the NDES connector with the new certificate.</span></span>
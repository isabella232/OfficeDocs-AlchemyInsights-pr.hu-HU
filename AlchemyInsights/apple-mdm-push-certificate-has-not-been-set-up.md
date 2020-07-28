---
title: Az Apple MDM leküldéses tanúsítványa nincs beállítva
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439382"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="1e463-102">Az Apple MDM leküldéses tanúsítványa nincs beállítva</span><span class="sxs-lookup"><span data-stu-id="1e463-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="1e463-103">Az Apple MDM leküldéses tanúsítványa (más néven Apple Push Notification Service (APNS) tanúsítvány) nincs konfigurálva az előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="1e463-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="1e463-104">Az Apple MDM leküldéses tanúsítványkonfigurálása nélkül nem tud iOS és Mac OS-eszközöket beállítani és kezelni.</span><span class="sxs-lookup"><span data-stu-id="1e463-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="1e463-105">Miután hozzáadja a tanúsítványt az Intune-hoz, a felhasználók telepíthetik a Céges portál alkalmazást az iOS-eszközök regisztrálásához.</span><span class="sxs-lookup"><span data-stu-id="1e463-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="1e463-106">Válassza az **"Egyetértek" lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="1e463-106">Select **"I agree."**</span></span> <span data-ttu-id="1e463-107">hogy a Microsoft engedélyt adjon az Apple-nek küldött adatok küldésére.</span><span class="sxs-lookup"><span data-stu-id="1e463-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="1e463-108">Válassza **az CSR letöltése** lehetőséget az Apple MDM leküldéses tanúsítvány létrehozásához szükséges Intune-tanúsítvány-aláíró kérelemre.</span><span class="sxs-lookup"><span data-stu-id="1e463-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="1e463-109">A fájl segítségével megbízhatósági kapcsolattanúsítványt kérhet az Apple Push Certificates Portal-tól.</span><span class="sxs-lookup"><span data-stu-id="1e463-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="1e463-110">Válassza **az MDM leküldéses tanúsítvány létrehozása lehetőséget** az Apple Push Certificates Portal megugrásához.</span><span class="sxs-lookup"><span data-stu-id="1e463-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="1e463-111">Jelentkezzen be a cégével, az Apple ID azonosítóval, és válassza **a Tanúsítvány létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="1e463-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="1e463-112">Válassza **a Fájl kiválasztása**lehetőséget, keresse meg a tanúsítványaláíró kérelemfájlt, majd válassza a **Feltöltés gombot.**</span><span class="sxs-lookup"><span data-stu-id="1e463-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="1e463-113">A Megerősítés lapon válassza a **Letöltés** gombot a tanúsítványfájl (.pem) letöltéséhez, majd a fájl helyi mentéséhez.</span><span class="sxs-lookup"><span data-stu-id="1e463-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="1e463-114">**Megjegyzés:** A tanúsítvány a létrehozásához használt Apple ID azonosítóhoz van társítva.</span><span class="sxs-lookup"><span data-stu-id="1e463-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="1e463-115">Ajánlott eljárásként használjon vállalati Apple ID azonosítót a felügyeleti feladatokhoz, és győződjön meg arról, hogy a postaládát egynél több személy vagy terjesztési lista használatával figyeli.</span><span class="sxs-lookup"><span data-stu-id="1e463-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="1e463-116">Soha ne használjon személyes Apple ID azonosítót.</span><span class="sxs-lookup"><span data-stu-id="1e463-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="1e463-117">Használja ugyanazt az Apple ID azonosítót az Apple Push tanúsítvány 12 havonta történő megújításához.</span><span class="sxs-lookup"><span data-stu-id="1e463-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="1e463-118">Adja meg az Apple MDM leküldéses tanúsítvány létrehozásához használt Apple ID azonosítót.</span><span class="sxs-lookup"><span data-stu-id="1e463-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="1e463-119">Rögzítse ezt az azonosítót emlékeztetőként, amikor meg kell újítania a tanúsítványt.</span><span class="sxs-lookup"><span data-stu-id="1e463-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="1e463-120">Nyissa meg a tanúsítványfájlt (.pem), válassza **a Megnyitás**lehetőséget, és válassza **a Feltöltés gombot.**</span><span class="sxs-lookup"><span data-stu-id="1e463-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="1e463-121">A leküldéses tanúsítvánnyal az Intune regisztrálhatja és kezelheti az Apple-eszközöket.</span><span class="sxs-lookup"><span data-stu-id="1e463-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>
---
title: Üzenettitkosítás konfigurálása hibrid környezetben
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745400"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="1e6f0-102">Üzenettitkosítás konfigurálása hibrid környezetben</span><span class="sxs-lookup"><span data-stu-id="1e6f0-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="1e6f0-103">Hibrid Exchange-környezetekben a helyszíni felhasználók csak akkor küldhetnek titkosított e-maileket az Office Üzenettitkosítás (OME) használatával, ha az e-maileket az Exchange Online-on keresztül irányítják át.</span><span class="sxs-lookup"><span data-stu-id="1e6f0-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="1e6f0-104">Az e-mailek OME-ben való titkosításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1e6f0-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="1e6f0-105">A hibrid [környezet beállítását a](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) Hibrid konfigurációs varázslóval használhatja.</span><span class="sxs-lookup"><span data-stu-id="1e6f0-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="1e6f0-106">A titkosítás beállításához nincs szükség speciális lépésekre.</span><span class="sxs-lookup"><span data-stu-id="1e6f0-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="1e6f0-107">[A szokásos módon állítson](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) be titkosítási szabályokat az e-mail-forgalomhoz.</span><span class="sxs-lookup"><span data-stu-id="1e6f0-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>



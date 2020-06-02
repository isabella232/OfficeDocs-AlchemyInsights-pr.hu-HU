---
title: S/MIME a Webes Outlookban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511510"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="d7325-102">E-mailek titkosítása az Outlookban</span><span class="sxs-lookup"><span data-stu-id="d7325-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="d7325-103">A Microsoft 365 üzenettitkosítás a Microsoft Azure Tartalomvédelmi Szolgáltatás (Azure RMS) szolgáltatásra épül, amely az Azure Information Protection része.</span><span class="sxs-lookup"><span data-stu-id="d7325-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="d7325-104">Ha előfizetése tartalmazza az Azure Rights Management vagy az Azure Information Protection szolgáltatást, nem kell semmilyen műveletet tennie a tartalomvédelmi szolgáltatás **manuális engedélyezéséhez vagy aktiválásához.**</span><span class="sxs-lookup"><span data-stu-id="d7325-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="d7325-105">Az ügyfelek visszajelzései alapján a továbbiakban nem engedélyezzük az Exchange levelezési szabályainak automatikus anno a bérlőben bizonyos típusú bizalmas adatokat tartalmazó kimenő e-mailek titkosítását.</span><span class="sxs-lookup"><span data-stu-id="d7325-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="d7325-106">Ehelyett részletes utasításokat adunk arra vonatkozóan, hogy ezt hogyan teheti meg.</span><span class="sxs-lookup"><span data-stu-id="d7325-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="d7325-107">A bizalmas adatok titkosítására szolgáló átviteli szabályok létrehozásáról a [cikkben](https://aka.ms/OmeEtr)olvashat további részletekről.</span><span class="sxs-lookup"><span data-stu-id="d7325-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="d7325-108">Ha a Webes Outlookot (korábbi ideig **OWA)** használja: E-mail írásakor egyszerűen kattintson a **Védelem** az OWA-ban gombra.</span><span class="sxs-lookup"><span data-stu-id="d7325-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="d7325-109">Ez a "Ne továbbítsa" engedélyt alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="d7325-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="d7325-110">Kattintson **a Módosítás gombra,** és válassza a **Titkosítás** lehetőséget az üzenet titkosításához.</span><span class="sxs-lookup"><span data-stu-id="d7325-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="d7325-111">**Outlook-ügyfél**használata esetén : Titkosított üzenet küldéséhez az Outlook 2013-ból vagy 2016-ból, illetve a Mac Outlook 2016-ból, válassza a **Beállítások**  >  **engedélyek**lehetőséget, majd válassza ki a szükséges védelmi beállítást.</span><span class="sxs-lookup"><span data-stu-id="d7325-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="d7325-112">Az egyes címzetteknek vagy külső partnerszervezeteknek küldött **összes e-mail automatikus titkosításához** létre kell hoznia egy levelezési átviteli szabályt az Exchange Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="d7325-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="d7325-113">Részletes utasításokat ebben a [támogatási cikkben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)talál.</span><span class="sxs-lookup"><span data-stu-id="d7325-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>


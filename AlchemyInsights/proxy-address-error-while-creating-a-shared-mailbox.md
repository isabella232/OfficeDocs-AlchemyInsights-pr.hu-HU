---
title: Proxycímhiba megosztott postaláda létrehozásakor
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568292"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="501eb-102">Proxycímhiba postaláda vagy más levelezési objektum létrehozása közben</span><span class="sxs-lookup"><span data-stu-id="501eb-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="501eb-103">Ha megpróbál létrehozni egy e-mail-kompatibilis objektumot (postaláda, megosztott postaláda stb.), és "A proxycím "SMTP:alias@domain.com" már használatban van..." hibaüzenet jelenik meg, akkor a választott e-mail-címet már a szervezet egy másik e-mail-képes objektuma hozza létre.</span><span class="sxs-lookup"><span data-stu-id="501eb-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="501eb-104">Meg kell találnia az e-mail-címet tartalmazó felhasználót, csoportot, megosztott postaládát vagy nyilvános mappát, és törölnie kell azt, vagy módosítania kell az e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="501eb-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="501eb-105">Ezután létrehozhat egy új, e-mail-címmel rendelkező objektumot a felszabadított e-mail címmel.</span><span class="sxs-lookup"><span data-stu-id="501eb-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="501eb-106">A kereséshez használja a Keresés lapot a kezdőlapon.</span><span class="sxs-lookup"><span data-stu-id="501eb-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="501eb-107">A következő Exchange Online PowerShell-paranccsal is megkeresheti:</span><span class="sxs-lookup"><span data-stu-id="501eb-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="501eb-108">Ha nem szeretné törölni a meglévő e-mail-címet, válasszon egy új e-mail-címet a létrehozott új objektumhoz.</span><span class="sxs-lookup"><span data-stu-id="501eb-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  
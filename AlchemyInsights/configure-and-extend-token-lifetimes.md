---
title: A jogkivonat élettartamának konfigurálása és meghosszabbítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916828"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="3bb95-102">A jogkivonat élettartamának konfigurálása és meghosszabbítása</span><span class="sxs-lookup"><span data-stu-id="3bb95-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="3bb95-103">Megadhatja a Microsoft identitásplatform által kibocsátott hozzáférési, SAML- vagy azonosítótokens élettartamát.</span><span class="sxs-lookup"><span data-stu-id="3bb95-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="3bb95-104">Beállíthatja a jogkivonat élettartamát a szervezet összes appja, egy több-bérlős (több szervezetből álló) alkalmazás vagy egy adott szolgáltatásnév számára a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="3bb95-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="3bb95-105">További információért olvassa el a [konfigurálható jogkivonat élettartamát.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="3bb95-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="3bb95-106">Példákat [a jogkivonat élettartamának beállítására vonatkozó példákban talál.](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="3bb95-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="3bb95-107">Ha tudni szeretne arról, hogy miként konfigurálhatja egy jogkivonat élettartamát és kompatibilitását az Azure Active Directory B2C szolgáltatásban (Azure AD B2C), olvassa el a Jogkivonatok konfigurálása az [Azure Active Directory B2C szolgáltatásban.](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)</span><span class="sxs-lookup"><span data-stu-id="3bb95-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="3bb95-108">A munkamenet viselkedésének konfigurálása az [Azure Active Directory B2C-ben](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) az Azure AD B2C-ben használt egyszeri bejelentkezési módszereket ismerteti, és segít a házirend konfigurálásához a legmegfelelőbb egyszeri bejelentkezési módszer választásában.</span><span class="sxs-lookup"><span data-stu-id="3bb95-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="3bb95-109">**Mennyi ideig tart a jogkivonat? Mennyi ideig érvényesek?**</span><span class="sxs-lookup"><span data-stu-id="3bb95-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="3bb95-110">A tokenek élettartama 1 óra, a munkamenet élettartama pedig 24 óra.</span><span class="sxs-lookup"><span data-stu-id="3bb95-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="3bb95-111">Ez azt jelenti, hogy ha 24 órán belül nem történt kérés, újra be kell jelentkeznie, mielőtt új jogkivonatot kér.</span><span class="sxs-lookup"><span data-stu-id="3bb95-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="3bb95-112">2020. május 30. után egy új bérlő sem fogja tudni használni a konfigurálható tokenek élettartam-házirendet a munkamenet és a tokenek frissítéséhez.</span><span class="sxs-lookup"><span data-stu-id="3bb95-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="3bb95-113">A felállás néhány hónapon belül megtörténik, ami azt jelenti, hogy a meglévő munkamenetet nem fogjuk tiszteletben hagyni, és frissítjük a jogkivonat-rendszerrendeket.</span><span class="sxs-lookup"><span data-stu-id="3bb95-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="3bb95-114">A lejárat után is konfigurálhatja a hozzáférési jogkivonat élettartamát.</span><span class="sxs-lookup"><span data-stu-id="3bb95-114">You can still configure access token lifetimes after the deprecation.</span></span>







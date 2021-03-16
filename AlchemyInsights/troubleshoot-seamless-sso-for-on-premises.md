---
title: A helyszíni egyszeri bejelentkezéssel kapcsolatos zökkenőmentes egyszeri bejelentkezés hibaelhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816208"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="a9d70-102">A helyszíni egyszeri bejelentkezéssel kapcsolatos zökkenőmentes egyszeri bejelentkezés hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="a9d70-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="a9d70-103">A zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák megoldásához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="a9d70-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="a9d70-104">**Hogyan tudom átgördülni az AZUREADSSO számítógépes fiók Kerberos-visszafejtési kulcsát?**</span><span class="sxs-lookup"><span data-stu-id="a9d70-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="a9d70-105">Azt javasoljuk, hogy legalább 30 naponta görgessen át a Kerberos-visszafejtési kulcson.</span><span class="sxs-lookup"><span data-stu-id="a9d70-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="a9d70-106">Ehhez lásd: A Kerberos-visszafejtési kulcsok [átváltása](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="a9d70-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="a9d70-107">**Gördülékeny egyszeri bejelentkezés beállítása**</span><span class="sxs-lookup"><span data-stu-id="a9d70-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="a9d70-108">A zökkenőmentes egyszeri bejelentkezés telepítéséhez kövesse Az Azure Active Directory zökkenőmentes egyszeri [bejelentkezés: Rövid útmutató lépéseit.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)</span><span class="sxs-lookup"><span data-stu-id="a9d70-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="a9d70-109">**Tanácsadói**</span><span class="sxs-lookup"><span data-stu-id="a9d70-109">**Advisory**</span></span>

- <span data-ttu-id="a9d70-110">[Azure Active Directory zökkenőmentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) egyszeri bejelentkezés: Gyakori kérdések – Ebben a cikkben az Azure Active Directory zökkenőmentes egyszeri bejelentkezési szolgáltatásának (SSO) gyakori kérdéseit Sign-On foglalkozunk.</span><span class="sxs-lookup"><span data-stu-id="a9d70-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="a9d70-111">Ellenőrizze újra az új tartalmakat.</span><span class="sxs-lookup"><span data-stu-id="a9d70-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="a9d70-112">[Microsoft kérdések&A –](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) Ez a cikk információt nyújt arról, hogy miként kérhet funkciókéréseket, illetve hogyan kérhet fel technikai kérdéseket a zökkenőmentes egyszeri bejelentkezésről.</span><span class="sxs-lookup"><span data-stu-id="a9d70-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="a9d70-113">**Hibaelhárítás**</span><span class="sxs-lookup"><span data-stu-id="a9d70-113">**Troubleshoot**</span></span>

<span data-ttu-id="a9d70-114">[Az Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) közvetlen egyszeri bejelentkezéssel kapcsolatos hibáinak elhárítása – Ez a cikk segítséget nyújt az Azure Active Directory (Azure AD) zökkenőmentes egyszeri bejelentkezési szolgáltatásával Sign-On kapcsolatos gyakori problémák hibaelhárításához.</span><span class="sxs-lookup"><span data-stu-id="a9d70-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>








---
title: E-mail-továbbítás a Microsoft 365-ön keresztül
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117985"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="6794e-102">Többfunkciós eszköz vagy alkalmazás beállítása levelek küldéséhez</span><span class="sxs-lookup"><span data-stu-id="6794e-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="6794e-103">A különféle lehetőségekről és az eljárás lépéseiről a [Többfunkciós eszköz vagy alkalmazás beállítása a Microsoft 365-tel való levelezéshez](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365) című cikk nyújt tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="6794e-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="6794e-104">Ha olyan eszköze vagy alkalmazása van, amely nemrég leállt, a leggyakoribb problémák a következők:</span><span class="sxs-lookup"><span data-stu-id="6794e-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="6794e-105">**Hitelesítéssel kapcsolatos hibák AZ SMTP Auth-ügyfélküldés használata során** Nemrégiben megváltoztattunk néhány, az SMTP-hitelesítés működését.</span><span class="sxs-lookup"><span data-stu-id="6794e-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="6794e-106">A problémák megoldásával kapcsolatos további információkért lásd: Az e-maileket levelező nyomtatókkal, szkennerekkel és hálózatolvasókkal kapcsolatos problémák megoldása a hitelesítés sikertelen Microsoft 365 [vagy](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)Office 365.</span><span class="sxs-lookup"><span data-stu-id="6794e-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="6794e-107">**A TLS 1.2-es** verzióját fogadjuk el, miközben biztonságos kapcsolatot létesítünk Office 365 Biztonságos kapcsolat (TLS) használata esetén győződjön meg arról, hogy az alkalmazáseszköz támogatja a TLS 1.2-es adatokat.</span><span class="sxs-lookup"><span data-stu-id="6794e-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="6794e-108">További információt a Felkészülés a [TLS 1.2-esre](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)a Office 365 és a Office 365 GCC.</span><span class="sxs-lookup"><span data-stu-id="6794e-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="6794e-109">Más problémákról és megoldásokról Az e-maileket levelező [nyomtatók,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)szkennerek éslobrák problémáinak megoldása Microsoft 365 vagy Office 365.</span><span class="sxs-lookup"><span data-stu-id="6794e-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="6794e-110">Az érintett eszközök megjelenítéséhez nyissa meg az [SMTP-hitelesítést használó ügyfelekről szóló jelentést](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="6794e-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="6794e-111">**Megjegyzés:** Exchange Online tömeges levelezési esetek nem használhatók.</span><span class="sxs-lookup"><span data-stu-id="6794e-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="6794e-112">Ha tömeges kereskedelmi e-maileket (például ügyfél hírleveleket) is el kell küldenie, külső szolgáltatót kell használnia, amely ezekre a szolgáltatásokra specializál.</span><span class="sxs-lookup"><span data-stu-id="6794e-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>

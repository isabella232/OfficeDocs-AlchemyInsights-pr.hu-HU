---
title: A TLS 1.0 és a TLS 1.1 letiltás miatt nem lehet e-maileket küldeni/fogadni az Office 365-be/
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745016"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="42075-102">A TLS 1.0 és a TLS 1.1 letiltás miatt nem lehet e-maileket küldeni/fogadni az Office 365-be/</span><span class="sxs-lookup"><span data-stu-id="42075-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="42075-103">Amint azt az MC229914-et, a TLS 1.0-s és a TLS 1.1-es elavultást követő üzenetközpont is igazolta, az Exchange Online levélforgalom végpontjainak kényszerítését kezdték meg.</span><span class="sxs-lookup"><span data-stu-id="42075-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="42075-104">Az Office 365 hamarosan nem fogadja el a külső forrásokból származó TLS 1.0-s és TLS 1.1-es e-mail-kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="42075-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="42075-105">Ezenkívül az Exchange Online soha nem használ TLS 1.0-s vagy 1.1-es portot a kimenő e-mailek küldését.</span><span class="sxs-lookup"><span data-stu-id="42075-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="42075-106">Ha a TLS 1.0-s vagy 1.1-es letiltása miatt problémákat tapasztal, az alábbi hibaüzenetek egyikét tapasztalhatja:</span><span class="sxs-lookup"><span data-stu-id="42075-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="42075-107">A feladó sikertelen kézbesítésről szóló jelentése visszapattan – '421 4.4.2 A Kapcsolat a SocketError miatt megszakadt'</span><span class="sxs-lookup"><span data-stu-id="42075-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="42075-108">Hiba a helyszíni kiszolgáló Várólistás megjelenítőben, amely a Officer 365-nek küld e-mailt – '421 4.4.2 A SocketError miatt megszakadt a kapcsolat"</span><span class="sxs-lookup"><span data-stu-id="42075-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="42075-109">A SocketError hiba [miatt](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) nem sikerült a TLS egyeztetése az Összekötők küldése naplóban a kiszolgálón, amely e-maileket küld az Office 365-be</span><span class="sxs-lookup"><span data-stu-id="42075-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="42075-110">Hiba az Összekötők küldése és fogadása protokollnaplóban – '451 5.7.3 KEZDÉSI PARANCS ki kell adva'</span><span class="sxs-lookup"><span data-stu-id="42075-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="42075-111">Ha a fenti hibák bármelyikét tapasztalja, az alábbi beállításkulcsok ellenőrzésével győződjön meg arról, hogy a TLS 1.2 engedélyezve van a TLS 1.2-es kiszolgálón.</span><span class="sxs-lookup"><span data-stu-id="42075-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="42075-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="42075-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="42075-113">Ha módosítja a fenti beállításkulcsokat a TLS 1.2 engedélyezéséhez, indítsa újra a kiszolgálót a módosítások érvénybe léptéhez.</span><span class="sxs-lookup"><span data-stu-id="42075-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="42075-114">Ellenőrizze azt is, hogy telepítve vannak-e a Windows és az Exchange legújabb frissítései.</span><span class="sxs-lookup"><span data-stu-id="42075-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="42075-115">További információ:</span><span class="sxs-lookup"><span data-stu-id="42075-115">For more information, see:</span></span>

- [<span data-ttu-id="42075-116">Exchange Server TLS – útmutató, 1. rész: A TLS 1.2-es verziójának készült készülő része – Microsoft technikai közösség</span><span class="sxs-lookup"><span data-stu-id="42075-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="42075-117">Az Exchange Server TLS 2. útmutatása: A TLS 1.2 engedélyezése és a nem használó ügyfelek azonosítása – Microsoft technikai közösség</span><span class="sxs-lookup"><span data-stu-id="42075-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="42075-118">A levelezési esetek ismertetése abban az esetben, ha nem lehet TLS-verziókat egyeztetni az Exchange Online-sal – Microsoft technikai közösség</span><span class="sxs-lookup"><span data-stu-id="42075-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)

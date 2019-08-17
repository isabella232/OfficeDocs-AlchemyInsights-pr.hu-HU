---
title: 305 archív postaláda méretének növelése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391329"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="fb66a-102">Az archív postaláda méretének növelése</span><span class="sxs-lookup"><span data-stu-id="fb66a-102">Increase the archive mailbox size</span></span>

<span data-ttu-id="fb66a-103">Office 365 [határértékek](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) alapján a licencet a felhasználói fiókhoz rendelt archív postaládák méretét.</span><span class="sxs-lookup"><span data-stu-id="fb66a-103">Office 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="fb66a-104">Az archív postaláda mérete megengedett mérete 90 %-át, amikor a felhasználó kap e-mailben értesítjük.</span><span class="sxs-lookup"><span data-stu-id="fb66a-104">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="fb66a-105">Az archív postaláda eléri a maximális méretét, ha a felhasználó nem további elemek áthelyezése az archív postaláda.</span><span class="sxs-lookup"><span data-stu-id="fb66a-105">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="fb66a-106">Az Office 365 nem az archív postaláda méretének növelése, amint elérik a maximális méretét.</span><span class="sxs-lookup"><span data-stu-id="fb66a-106">Office 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="fb66a-107">Ehelyett a felhasználók az archív postaládában helyet szabadíthat fel a következő műveletek hajthatók végre:</span><span class="sxs-lookup"><span data-stu-id="fb66a-107">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="fb66a-108">Exportálja a az elemeket egy .pst fájl az Outlook programmal</span><span class="sxs-lookup"><span data-stu-id="fb66a-108">Export the the items to a .pst file using Outlook</span></span>

- <span data-ttu-id="fb66a-109">Elemek törlése az archív postaláda.</span><span class="sxs-lookup"><span data-stu-id="fb66a-109">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="fb66a-110">Office 365 biztosít **korlátlan archiválási** Office 365 vállalati E3, E5 és licencek.</span><span class="sxs-lookup"><span data-stu-id="fb66a-110">Office 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="fb66a-111">Egy rendszergazda engedélyezni kell a szolgáltatást, mielőtt az archív postaláda eléri a maximális méretét.</span><span class="sxs-lookup"><span data-stu-id="fb66a-111">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="fb66a-112">Ha korlátlan archiválási engedélyezve van, legfeljebb 30 nappal megelőzően szabad lemezterület hozzáadódik az archív postaláda is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="fb66a-112">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="fb66a-113">Emiatt javasoljuk, hogy a rendszergazdák ellenőrizze a szabad lemezterület a postafiók archívum, amely lehetővé teszi a felhasználó továbbra is használni az archív postaláda, miközben bővíti.</span><span class="sxs-lookup"><span data-stu-id="fb66a-113">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="fb66a-114">További információt talál [az Office 365 rendszerben korlátlan archiválási áttekintése](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) és [az Office 365 rendszerben korlátlan archiválásának engedélyezése](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)</span><span class="sxs-lookup"><span data-stu-id="fb66a-114">For more information, see [Overview of unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) and [Enable unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="fb66a-115">Az Outlook programból az archív postaláda elérésével kapcsolatban további információt lásd: [Outlook követelmények eléréséhez szükséges elemek automatikus bővített archívumot](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span><span class="sxs-lookup"><span data-stu-id="fb66a-115">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="fb66a-116">Adja meg egy adatmegőrzési szabályt, amely automatikusan átmozgatja a cikkeket az archív postaládába, olvassa el [az Office 365 szervezetben postafiókok archív és törlés házirend beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="fb66a-116">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Office 365 organization](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="fb66a-117">**Megjegyzés**: meghagyni archívumok elsődleges postafiókok Exchange 2010 nem támogatja.</span><span class="sxs-lookup"><span data-stu-id="fb66a-117">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
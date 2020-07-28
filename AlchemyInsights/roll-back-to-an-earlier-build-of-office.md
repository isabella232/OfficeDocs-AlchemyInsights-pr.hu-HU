---
title: Visszaállítás az Office egy korábbi buildjéhez
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 8c7d019ec1aa6c26cffebbcd2c3e5751c853e3a4
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439564"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="c27b8-102">Visszaállítás az Office egy korábbi buildjéhez</span><span class="sxs-lookup"><span data-stu-id="c27b8-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="c27b8-103">A Microsoft 365 alkalmazások korábbi buildjéhez vagy verziójához való visszatéréshez olvassa el [Az Office korábbi verziójának visszaállítása](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic)című témakört.</span><span class="sxs-lookup"><span data-stu-id="c27b8-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="c27b8-104">Ha váltani szeretne az egyik Microsoft 365-előfizetésről a másikra, olvassa el [a Váltás másik Microsoft 365 vállalati verziós csomagra](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="c27b8-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="c27b8-105">A jelenleg használt Office-verzió megkereséséhez olvassa el [Az Office milyen verzióját használom?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)</span><span class="sxs-lookup"><span data-stu-id="c27b8-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="c27b8-106">A visszagörgetni kívánt build meghatározásáról a [Microsoft 365-alkalmazások előzményei (dátum szerint felsorolásban)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7)című témakörben találja.</span><span class="sxs-lookup"><span data-stu-id="c27b8-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="c27b8-107">Állítsa be a **TargetVersion** beállítást úgy, hogy visszatérjen a korábbi buildhez az [Office korábbi verziójának visszaállítása](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) vagy [a Szolgáltatásfrissítések fogadásának késleltetése féléves csatornáról az Office Content Delivery Network (CDN) használatakor](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn)használatával.</span><span class="sxs-lookup"><span data-stu-id="c27b8-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="c27b8-108">Ha a célverzió be van állítva, az Office a frissítések következő keresésekor frissül az adott verzióra.</span><span class="sxs-lookup"><span data-stu-id="c27b8-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>
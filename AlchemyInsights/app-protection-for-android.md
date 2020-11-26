---
title: Az Android app Protection Policy beállításai a Microsoft Intune-ban
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003997"
- "7057"
ms.openlocfilehash: 327df6e0a901037cd929cb845f805466d9bd4eff
ms.sourcegitcommit: 81c86027933c06db08d264918f2698d9c9a1659a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/20/2020
ms.locfileid: "49447412"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a><span data-ttu-id="af186-102">Az Android app Protection Policy beállításai a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="af186-102">Android app protection policy settings in Microsoft Intune</span></span>

<span data-ttu-id="af186-103">Az App Protection Policy beállításai az Android-eszközökhöz három kategóriába sorolhatók:</span><span class="sxs-lookup"><span data-stu-id="af186-103">There are three categories of app protection policy settings for Android devices:</span></span>

<span data-ttu-id="af186-104">**Az adatvédelem szabályozza a** vállalati adatkezelési módokat, például hogy az adatmásolható vagy beilleszthető-e egy másik alkalmazásba, illetve hogy van-e képernyőkép az alkalmazásról.</span><span class="sxs-lookup"><span data-stu-id="af186-104">**Data protection** controls how company data is handled, such as, whether data can be copied or pasted to a different app or whether a screenshot can be taken of the app.</span></span> <span data-ttu-id="af186-105">A beállítások a vállalati adatok titkosítását is kikényszerítik, és kezelik, hogy bizonyos adatok szinkronizálva legyenek-e a natív eszköz alkalmazásaival, például a partnerlista vagy a webböngésző használatával.</span><span class="sxs-lookup"><span data-stu-id="af186-105">The settings also enforce encryption on company data and manage whether certain data can be synced with the native device apps, like the contact list or web browser.</span></span> <span data-ttu-id="af186-106">További információt az [Adatvédelem](https://go.microsoft.com/fwlink/?linkid=2135259)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="af186-106">To learn more, see [Data protection](https://go.microsoft.com/fwlink/?linkid=2135259).</span></span>

<span data-ttu-id="af186-107">A **hozzáférési követelményekkel** a felhasználók elérheti az alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="af186-107">**Access requirements** guides how users can access an app.</span></span> <span data-ttu-id="af186-108">Egy alkalmazásban például szükség lehet arra, hogy a felhasználó PIN-kódot vagy ujjlenyomatot írjon az eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="af186-108">For example, an app could require the user to enter a PIN or fingerprint to access it.</span></span> <span data-ttu-id="af186-109">További információt a [hozzáférési követelmények](https://go.microsoft.com/fwlink/?linkid=2135260)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="af186-109">To learn more, see [Access requirements](https://go.microsoft.com/fwlink/?linkid=2135260).</span></span>

<span data-ttu-id="af186-110">A **feltételes indítás** szabályozza az alkalmazások bejelentkezési biztonsági beállításait, például a zárolás előtti maximális kísérleteket, illetve az alkalmazás futtatásához szükséges minimális operációs rendszert.</span><span class="sxs-lookup"><span data-stu-id="af186-110">**Conditional launch** governs the sign-in security settings for an app, such as, the maximum PIN attempts before lockout or the minimum operating system needed to run the app.</span></span> <span data-ttu-id="af186-111">További információt a [feltételes indítás](https://go.microsoft.com/fwlink/?linkid=2135507)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="af186-111">To learn more, see [Conditional launch](https://go.microsoft.com/fwlink/?linkid=2135507).</span></span>

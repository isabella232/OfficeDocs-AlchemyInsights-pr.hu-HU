---
title: A Microsoft Graph API lekérdezése
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974420"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="cdf2b-102">A Microsoft Graph API lekérdezése</span><span class="sxs-lookup"><span data-stu-id="cdf2b-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="cdf2b-103">Ez a témakör az Azure AD Graph API-t még használó fejlesztőkre is vonatkozhat.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="cdf2b-104">Erősen javasoljuk **azonban,** hogy a Microsoft Graphot minden címtár-, identitás- és hozzáférés-kezelési esethez használja.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="cdf2b-105">**Hitelesítési vagy engedélyezési problémák**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="cdf2b-106">Ha az  app nem tud jogkivonatokat szerezni a Microsoft Graph hívásához, válassza a Microsoft Graph-kategória Hozzáférési jogkivonat **(Hitelesítés)** esetén a probléma megoldását, ha további segítségre és támogatásra van szüksége a témakörben.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="cdf2b-107">Ha az app **401-es vagy 403-as** engedélyezési hibát kap a Microsoft Graph hívása közben, válassza a Hozzáférés megtagadva **(Engedélyezés)** Microsoft Graph API-kategóriát, ha további konkrét segítséget és támogatást kap erről a témakörről.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="cdf2b-108">**A Microsoft Graphot szeretném használni, de nem tudom, hol kezdjem**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="cdf2b-109">A Microsoft Graphról az alábbi cikkből olvashat bővebben:</span><span class="sxs-lookup"><span data-stu-id="cdf2b-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="cdf2b-110">A Microsoft Graph áttekintése</span><span class="sxs-lookup"><span data-stu-id="cdf2b-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="cdf2b-111">Az identitás- és hozzáférés-kezelés áttekintése a Microsoft Graphban</span><span class="sxs-lookup"><span data-stu-id="cdf2b-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="cdf2b-112">Microsoft Graph-alkalmazások építésének első lépések</span><span class="sxs-lookup"><span data-stu-id="cdf2b-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="cdf2b-113">**Microsoft Graph Explorer** – A Microsoft Graph API-k tesztelése a bérlői vagy a bemutató bérlői webhelyen</span><span class="sxs-lookup"><span data-stu-id="cdf2b-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="cdf2b-114">**Szeretném használni a Microsoft Graphot, de támogatja a szükséges v1.0-s címtár API-kat?**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="cdf2b-115">A Microsoft Graph a címtár- és identitáskezeléshez, valamint a hozzáférés-kezeléshez ajánlott API.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="cdf2b-116">Az Azure AD Graph és a Microsoft Graph szolgáltatásai között azonban továbbra is van néhány hiányosságok.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="cdf2b-117">Tekintse át az alábbi cikkeket, amelyek kiemelik a legfrissebb különbségeket, hogy segítsék a választást:</span><span class="sxs-lookup"><span data-stu-id="cdf2b-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="cdf2b-118">Erőforrástípusbeli különbségek az Azure AD Graph és a Microsoft Graph között</span><span class="sxs-lookup"><span data-stu-id="cdf2b-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="cdf2b-119">Az Azure AD Graph és a Microsoft Graph közötti tulajdonságkülönbségek</span><span class="sxs-lookup"><span data-stu-id="cdf2b-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="cdf2b-120">Módszerbeli különbségek az Azure AD és a Microsoft Graph között</span><span class="sxs-lookup"><span data-stu-id="cdf2b-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="cdf2b-121">**Amikor lekérdezem *a felhasználói* objektumot, számos tulajdonsága hiányzik**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="cdf2b-122">`GET https://graph.microsoft.com/v1.0/users`csak 11 tulajdonságot ad vissza, mivel a  Microsoft Graph automatikusan kiválasztja a visszaadni kívánt alapértelmezett felhasználói tulajdonságokat.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="cdf2b-123">Ha más felhasználói *tulajdonságokra* van szüksége, $select az alkalmazás igényeinek megfelelő tulajdonságokat.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="cdf2b-124">Először próbálja ki a **Microsoft Graph Explorerben.**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="cdf2b-125">**Egyes felhasználói tulajdonságértékek *null értékűek* annak ellenére, hogy tudom, hogy be vannak állítva**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="cdf2b-126">A legvalószínűbb magyarázat az, hogy az alkalmazás a *User.ReadBasic.All* engedélyt is megadta.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="cdf2b-127">Ez lehetővé teszi, hogy az alkalmazás beolvassa a felhasználói tulajdonságok egy bizonyos készletét, és az összes többi tulajdonságot null értékként adja vissza, még akkor is, ha korábban be vannak állítva.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="cdf2b-128">Próbálja meg ehelyett *a User.Read.All* engedélyt kiadó alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="cdf2b-129">További információt a [Microsoft Graph felhasználói engedélyeiben található.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="cdf2b-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="cdf2b-130">**Problémáim vannak az OData-lekérdezési paraméterek használatával a kérések adatainak szűréséhez**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="cdf2b-131">Bár a Microsoft Graph az OData-lekérdezési paraméterek széles körét támogatja, a Microsoft Graph címtárszolgáltatásai (a *címtárobjektumtól öröklött* erőforrások) nem támogatják teljes mértékben ezeket a paramétereket.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="cdf2b-132">Az Azure AD Graph-ban ugyanazok a korlátozások maradnak meg, amelyek a Legtöbb esetben a Microsoft Graphban is fennállnak:</span><span class="sxs-lookup"><span data-stu-id="cdf2b-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="cdf2b-133">**Nem támogatott:**$count, $search és $filter *null* vagy nem *null érték esetén*</span><span class="sxs-lookup"><span data-stu-id="cdf2b-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="cdf2b-134">**Nem támogatott:**$filter tulajdonságokon (lásd az erőforrásokkal kapcsolatos témaköröket, amelyeken szűrhető tulajdonságok vannak)</span><span class="sxs-lookup"><span data-stu-id="cdf2b-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="cdf2b-135">**Nem támogatott:** egyszerre lapozás, szűrés és rendezés</span><span class="sxs-lookup"><span data-stu-id="cdf2b-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="cdf2b-136">**Nem támogatott:** kapcsolat szűrése.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="cdf2b-137">Megkeresheti például az Egyesült Királyságban található mérnöki csoport összes tagját.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="cdf2b-138">**Részleges támogatás:**$orderby *felhasználón* (displayName és userPrincipalName csak) és *csoporton*</span><span class="sxs-lookup"><span data-stu-id="cdf2b-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="cdf2b-139">Részleges **támogatás:**$filter (csak *eq*, *kezdetek,* *vagy*, és *,* és *korlátozott)* támogatás, az $expand (egyetlen objektum kapcsolatának kibontása visszaadja az összes kapcsolatot, de az objektumok kapcsolatainak kibontása korlátozott)</span><span class="sxs-lookup"><span data-stu-id="cdf2b-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="cdf2b-140">További információt a válaszok [testreszabása lekérdezési paraméterekkel.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="cdf2b-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="cdf2b-141">**A híváshoz hívott API nem működik – hol lehet további teszteket tesztelni?**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="cdf2b-142">**Microsoft Graph Explorer** – Tesztelje a Microsoft Graph API-kat  a bérlői vagy a demo bérlői fiókjában, és tekintse meg a Minta lekérdezéseket a Microsoft Graph Explorerben.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="cdf2b-143">**Adatok lekérdezésekor úgy tűnik, hiányos adatok halmazát kapom vissza**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="cdf2b-144">Ha egy gyűjteményt (például a felhasználókat) lekérdezést *használ,* a Microsoft Graph kiszolgálóoldali lapkorlátokat használ, így az eredmények mindig alapértelmezett oldalmérettel nyomtatódnak vissza.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="cdf2b-145">Az alkalmazásnak mindig a szolgáltatásból visszaadott gyűjtemények lapjára kell számítania.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="cdf2b-146">További információ:</span><span class="sxs-lookup"><span data-stu-id="cdf2b-146">For more information, see:</span></span>

- [<span data-ttu-id="cdf2b-147">Ajánlott eljárások a Microsoft Graphhoz</span><span class="sxs-lookup"><span data-stu-id="cdf2b-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="cdf2b-148">Microsoft Graph-adatok lapozása az alkalmazásban</span><span class="sxs-lookup"><span data-stu-id="cdf2b-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="cdf2b-149">**Az app túl lassú, és le van szabályozás alatt. Milyen fejlesztéseket tudok tenni?**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="cdf2b-150">A helyzettől függően számos különböző lehetőség áll a rendelkezésére az alkalmazás végrehajtásához, és bizonyos esetekben kevésbé van kivetve a szolgáltatás szabályozásának (ha túl sok hívást kezdeményez).</span><span class="sxs-lookup"><span data-stu-id="cdf2b-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="cdf2b-151">További információt az alábbi témakörökben találhat:</span><span class="sxs-lookup"><span data-stu-id="cdf2b-151">To learn more, see:</span></span>

- [<span data-ttu-id="cdf2b-152">Ajánlott eljárások a Microsoft Graphhoz</span><span class="sxs-lookup"><span data-stu-id="cdf2b-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="cdf2b-153">Kötegkérések</span><span class="sxs-lookup"><span data-stu-id="cdf2b-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="cdf2b-154">Változások követése a különbözeti lekérdezésen keresztül</span><span class="sxs-lookup"><span data-stu-id="cdf2b-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="cdf2b-155">Értesítés a változásokról webhookokon keresztül</span><span class="sxs-lookup"><span data-stu-id="cdf2b-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="cdf2b-156">Szabályozási útmutató</span><span class="sxs-lookup"><span data-stu-id="cdf2b-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="cdf2b-157">**Hol találok további információt a hibákról és az ismert problémákról?**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="cdf2b-158">A Microsoft Graph hibare adott válaszokkal kapcsolatos adatai</span><span class="sxs-lookup"><span data-stu-id="cdf2b-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="cdf2b-159">A Microsoft Graph ismert problémái</span><span class="sxs-lookup"><span data-stu-id="cdf2b-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="cdf2b-160">**Hol tudom ellenőrizni a szolgáltatás elérhetőségét és csatlakozását?**</span><span class="sxs-lookup"><span data-stu-id="cdf2b-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="cdf2b-161">A Microsoft Graphon keresztül elérhető mögöttes szolgáltatások elérhetősége és csatlakozása hatással lehet a Microsoft Graph általános elérhetőségére és teljesítményére.</span><span class="sxs-lookup"><span data-stu-id="cdf2b-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="cdf2b-162">Az Azure Active Directory szolgáltatásállapota esetén ellenőrizze az Azure állapotlapján felsorolt **Biztonsági és** identitásszolgáltatások [állapotát.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="cdf2b-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="cdf2b-163">A Microsoft Graph-hoz hozzájáruló Office-szolgáltatások állapotát az Office szolgáltatásállapot-irányítópultján [ellenőrizheti.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="cdf2b-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

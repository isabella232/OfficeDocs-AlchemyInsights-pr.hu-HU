---
title: A szervezeti globális címlista és az offline címjegyzék kezelése
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
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794834"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="5b46b-102">A szervezeti globális címlista (GAL) és az offline címjegyzék (OAB) kezelése</span><span class="sxs-lookup"><span data-stu-id="5b46b-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="5b46b-103">A globális címlista (GAL) a szervezet levelezésre alkalmas objektumainak (e-mail fogadására képes bármilyen típusú címzettjeinek) listája.</span><span class="sxs-lookup"><span data-stu-id="5b46b-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="5b46b-104">A rendszer mindegyik szervezetben automatikusan létrehoz egy globális címlistát.</span><span class="sxs-lookup"><span data-stu-id="5b46b-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="5b46b-105">Létrehozhat további globális címlistákat, ha szeretné szervezet vagy hely szerint különválasztani a felhasználókat, de egy adott felhasználó egyszerre csak egy globális címlistát láthat és használhat.</span><span class="sxs-lookup"><span data-stu-id="5b46b-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="5b46b-106">Egyes levelezőprogramok – például a Windows Outlook – letöltik a globális címlistát offline használatra.</span><span class="sxs-lookup"><span data-stu-id="5b46b-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="5b46b-107">Ez a letöltött címlista az offline címjegyzék (OAB).</span><span class="sxs-lookup"><span data-stu-id="5b46b-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="5b46b-108">Az Exchange Online-ban egy offline címjegyzék mindössze 8 óránként frissül, és utána az ügyfeleknek le kell tölteniük, hogy frissítsék az offline címjegyzékük helyi példányát.</span><span class="sxs-lookup"><span data-stu-id="5b46b-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="5b46b-109">A címzettek mindennemű módosításának először a globális címlistán kell megjelennie, hogy később bekerüljön az offline címjegyzékbe.</span><span class="sxs-lookup"><span data-stu-id="5b46b-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="5b46b-110">Alább felsorolunk néhány, a globális címlistával és az offline címjegyzékkel kapcsolatos gyakori eljárást:</span><span class="sxs-lookup"><span data-stu-id="5b46b-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="5b46b-111">Számos különböző ok miatt előfordulhat, hogy el szeretne rejteni egyes objektumokat a globális címlistáról.</span><span class="sxs-lookup"><span data-stu-id="5b46b-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="5b46b-112">Ehhez tekintse át a [Címzettek elrejtése címlistákról](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists) című témakört.</span><span class="sxs-lookup"><span data-stu-id="5b46b-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="5b46b-113">Ha testreszabott nézeteket kell biztosítania a szervezet globális címlistájáról a felhasználók meghatározott csoportjai számára, olvassa el a [Címjegyzék-házirendek az Exchange Online-ban](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies) című témakört.</span><span class="sxs-lookup"><span data-stu-id="5b46b-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="5b46b-114">[Hozzon létre egy globális címlistát az Exchange Online-ban](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), és ismerkedjen meg a globális címlistákra vonatkozó engedélyek használatával, ehhez tekintse át a [Címlisták az Exchange Online-ban](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) című témakört.</span><span class="sxs-lookup"><span data-stu-id="5b46b-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="5b46b-115">Felhívjuk a figyelmét arra, hogy új globális címlista létrehozása esetén célszerű lehet egy új offline címjegyzéket is létrehozni.</span><span class="sxs-lookup"><span data-stu-id="5b46b-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="5b46b-116">Erről [Az offline címjegyzékkel kapcsolatos eljárások](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures) című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="5b46b-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>

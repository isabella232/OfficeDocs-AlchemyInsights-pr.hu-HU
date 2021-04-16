---
title: Írás írásra megnyitott fájl
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813186"
---
# <a name="file-open-read-only"></a><span data-ttu-id="81e03-102">Írás írásra megnyitott fájl</span><span class="sxs-lookup"><span data-stu-id="81e03-102">File open read-only</span></span>

<span data-ttu-id="81e03-103">Előfordulhat, hogy a fájlok megnyitásakor a megnyitásuk csak olvashatóként történik.</span><span class="sxs-lookup"><span data-stu-id="81e03-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="81e03-104">Bizonyos esetekben ez a nagyobb biztonság érdekében van így, például amikor az internetről nyit meg fájlokat, más esetekben pedig egy módosítható beállítás miatt.</span><span class="sxs-lookup"><span data-stu-id="81e03-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="81e03-105">Íme néhány eset, amikor egy fájl csak olvashatóként nyílik meg, és néhány lépéssel módosíthatja azt.</span><span class="sxs-lookup"><span data-stu-id="81e03-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="81e03-106">**A víruskereső miatt csak olvashatóan nyílik meg a fájl**</span><span class="sxs-lookup"><span data-stu-id="81e03-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="81e03-107">Egyes víruskereső programok írásra megnyitva védhetnek a potenciálisan nem biztonságos fájlok ellen.</span><span class="sxs-lookup"><span data-stu-id="81e03-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="81e03-108">Előfordulhat, hogy a beállítások módosításához a víruskereső szolgáltatójától kell tájékozódni.</span><span class="sxs-lookup"><span data-stu-id="81e03-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="81e03-109">A BitDefender például az alkalmazáskizárások hozzáadásáról a következő tartalommal rendelkezik: Alkalmazás- vagy folyamatkizárások hozzáadása a [Bitdefender vezérlőközpontjában.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="81e03-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="81e03-110">**Írásra van-e állítva a fájltulajdonságok?**</span><span class="sxs-lookup"><span data-stu-id="81e03-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="81e03-111">A fájl tulajdonságainak ellenőrzéshez kattintson a jobb gombbal a fájlra, és válassza a Tulajdonságok parancsot.</span><span class="sxs-lookup"><span data-stu-id="81e03-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="81e03-112">Ha be van jelölve a Csak olvasható attribútum, törölje a jelölését, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="81e03-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="81e03-113">**A tartalom védett nézetben van**</span><span class="sxs-lookup"><span data-stu-id="81e03-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="81e03-114">Az internetről és más, potenciálisan nem biztonságos helyekről származó fájlok a számítógépet kártékony vírusokat, férgeket vagy más típusú kártevőket tartalmazhatnak.</span><span class="sxs-lookup"><span data-stu-id="81e03-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="81e03-115">Általában ez a helyzet az e-mail mellékletek és a letöltött fájlok esetében is.</span><span class="sxs-lookup"><span data-stu-id="81e03-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="81e03-116">A számítógép védelme érdekében az ilyen, potenciálisan nem biztonságos helyekről származó fájlok védett nézetben nyithatók meg.</span><span class="sxs-lookup"><span data-stu-id="81e03-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="81e03-117">A védett nézet használatával úgy olvashatja el a fájlokat és megtekintheti a tartalmát, hogy közben csökkenti a kockázatokat.</span><span class="sxs-lookup"><span data-stu-id="81e03-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="81e03-118">A védett nézetről és a beállítások módosításáról a következő cikkben olvashat bővebben: Mi [a védett nézet?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="81e03-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="81e03-119">**Megtelt a OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="81e03-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="81e03-120">Ha a fájlt a OneDrive-on tárolja, és megtelt a OneDrive-tárterülete, akkor mindaddig nem fogja tudni menteni a dokumentumot, amíg a kiosztott tárterület alá nem áll.</span><span class="sxs-lookup"><span data-stu-id="81e03-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="81e03-121">A OneDrive-on a szabad terület ellenőrzéséhez kattintson a OneDrive ikonra az értesítési központban, és válassza a Tárterület kezelése gombra kattintva, vagy a ikonra kattintva jelentkezzen be, és jegyezze fel a felhasznált terület mennyiségét a képernyő bal alsó [https://onedrive.live.com](https://onedrive.live.com) részén.</span><span class="sxs-lookup"><span data-stu-id="81e03-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="81e03-122">**Aktiválva van az Office?**</span><span class="sxs-lookup"><span data-stu-id="81e03-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="81e03-123">Ha az Office nincs aktiválva, vagy ha lejárt az előfizetése, akkor lehet, hogy csak olvasható csökkentett szolgáltatáskészletű üzemmódban van.</span><span class="sxs-lookup"><span data-stu-id="81e03-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="81e03-124">Az Office aktiválásának mikéntjére vonatkozó információkért lásd: "Nem licencelt termék" aktiválási hibaüzenetek az [Office-ban.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="81e03-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="81e03-125">**Ha minden más kudarcotik...**</span><span class="sxs-lookup"><span data-stu-id="81e03-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="81e03-126">Próbálkozzon a számítógép újraindításával</span><span class="sxs-lookup"><span data-stu-id="81e03-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="81e03-127">Office-frissítések telepítése</span><span class="sxs-lookup"><span data-stu-id="81e03-127">Install Office updates</span></span>
    
- <span data-ttu-id="81e03-128">Az Office online javítása</span><span class="sxs-lookup"><span data-stu-id="81e03-128">Perform an Online repair of Office</span></span>
    


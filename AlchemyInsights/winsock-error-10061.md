---
title: 1554 Winsock kesalahan 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772445"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="2ee26-102">Winsock kesalahan 10061</span><span class="sxs-lookup"><span data-stu-id="2ee26-102">Winsock error 10061</span></span>

<span data-ttu-id="2ee26-103">Kode kesalahan ini berarti bahwa Office 365 tidak bisa membangun soket TCP (koneksi) dengan target host.</span><span class="sxs-lookup"><span data-stu-id="2ee26-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="2ee26-104">Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda.</span><span class="sxs-lookup"><span data-stu-id="2ee26-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="2ee26-105">Untuk mengatasi masalah, periksa pengaturan ini:</span><span class="sxs-lookup"><span data-stu-id="2ee26-105">To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="2ee26-106">Memverifikasi Konfigurasi firewall Anda dengan informasi di [kantor 365 URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2ee26-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="2ee26-107">Jika kesalahan tertentu untuk perlindungan Online pertukaran (EOP), Anda harus telah sebelumnya diberitahu untuk perubahan [Alamat IP perlindungan Online pertukaran](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2ee26-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="2ee26-108">Pastikan bahwa Anda Internet Service Provider (ISP) tidak memblokir port.</span><span class="sxs-lookup"><span data-stu-id="2ee26-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="2ee26-109">Pastikan pengaturan server host dan target cerdas dalam konektor Anda.</span><span class="sxs-lookup"><span data-stu-id="2ee26-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="2ee26-110">Perhatikan bahwa Office 365 tidak memblokir koneksi *masuk* dengan cara ini.</span><span class="sxs-lookup"><span data-stu-id="2ee26-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

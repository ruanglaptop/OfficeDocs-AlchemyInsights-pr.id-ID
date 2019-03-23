---
title: Alamat 1065 bantahan EOP outbound IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777275"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="ea322-102">Bantahan dari EOP kisaran alamat IP keluar</span><span class="sxs-lookup"><span data-stu-id="ea322-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="ea322-103">Kami telah mendeteksi potensi masalah dengan organisasi yang (jika tidak diperbaiki oleh 26 Oktober 2018) mungkin istirahat alur e-mail ke lokal atau tujuan eksternal.</span><span class="sxs-lookup"><span data-stu-id="ea322-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="ea322-104">Sebagaimana diwartakan sebelumnya, untuk menyederhanakan manajemen kisaran alamat IP, kita sedang mengkonsolidasikan rentang alamat IP perlindungan Online pertukaran (EOP) yang digunakan untuk mengirim dan menerima email di luar Office 365.</span><span class="sxs-lookup"><span data-stu-id="ea322-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="ea322-105">Analisis kami menunjukkan bahwa satu atau lebih email eksternal sumber atau tujuan yang dikonfigurasi di mail aliran konektor tidak menerima koneksi dari IP alamat rentang ditunjukkan [di sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ea322-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="ea322-106">Bertindak sebelum Oktober 26 untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua [diterbitkan alamat EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ea322-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="ea322-107">Untuk informasi lebih lanjut mengenai perubahan ini, lihat pusat pesan posting [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="ea322-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="ea322-108">**Catatan**: jika Anda sebelumnya menggunakan IP atau URL penerbitan melalui HTML, XML, dan RSS pembaruan endpoint, Anda juga harus memigrasi ke layanan web baru untuk mengotomatisasi jenis update.</span><span class="sxs-lookup"><span data-stu-id="ea322-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="ea322-109">Untuk informasi lebih lanjut, lihat [kategori endpoint Office 365 dan kantor 365 alamat IP dan URL web layanan](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="ea322-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

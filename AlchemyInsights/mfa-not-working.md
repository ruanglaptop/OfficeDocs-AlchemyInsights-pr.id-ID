---
title: Masalah dengan MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250168"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="62229-102">Masalah dengan MFA</span><span class="sxs-lookup"><span data-stu-id="62229-102">Issues with MFA</span></span>
<span data-ttu-id="62229-103">Ada beberapa hal untuk memeriksa jika pengguna tidak dapat login menggunakan multi faktor otentikasi (MFA)</span><span class="sxs-lookup"><span data-stu-id="62229-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="62229-104">Terkena pengguna dapat diblokir di Azure Portal direktori aktif.</span><span class="sxs-lookup"><span data-stu-id="62229-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="62229-105">Jika itu terjadi, otentikasi upaya untuk itu pengguna akan secara otomatis ditolak.</span><span class="sxs-lookup"><span data-stu-id="62229-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="62229-106">Ikuti langkah-langkah dalam artikel ini untuk mereka.</span><span class="sxs-lookup"><span data-stu-id="62229-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="62229-107">Jika blokir pengguna tidak membantu atau pengguna tidak diblokir Anda dapat mencoba untuk me-reset MFA untuk pengguna dan mereka akan pergi melalui proses pendaftaran lagi.</span><span class="sxs-lookup"><span data-stu-id="62229-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="62229-108">Ikuti langkah-langkah dalam artikel ini.</span><span class="sxs-lookup"><span data-stu-id="62229-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="62229-109">Jika ini adalah pertama kali Anda diaktifkan MFA dan pengguna tidak dapat login untuk klien bebas-browser seperti Outlook, Skype, dll, mungkin ADAL (Active Directory otentikasi Perpustakaan) tidak diaktifkan pada kepelangganan O365.</span><span class="sxs-lookup"><span data-stu-id="62229-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="62229-110">Dalam hal ini Anda akan perlu untuk menyambung ke Exchange Online Powershell dan menjalankan cmdlet ini:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="62229-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
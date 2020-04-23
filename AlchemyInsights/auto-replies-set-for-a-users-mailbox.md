---
title: Mengatur balasan otomatis untuk kotak surat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509505"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="5fbf5-102">Mengatur balasan otomatis untuk kotak surat pengguna</span><span class="sxs-lookup"><span data-stu-id="5fbf5-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="5fbf5-103">**Metode 1**</span><span class="sxs-lookup"><span data-stu-id="5fbf5-103">**Method 1**</span></span>

1. <span data-ttu-id="5fbf5-104">Masuk ke portal Office 365.</span><span class="sxs-lookup"><span data-stu-id="5fbf5-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="5fbf5-105">Masuk ke **Pengguna > Pengguna aktif** (atau **Grup > Kotak surat bersama** jika Anda menetapkannya di kotak surat bersama).</span><span class="sxs-lookup"><span data-stu-id="5fbf5-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="5fbf5-106">Pilih pengguna yang memiliki kotak surat Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fbf5-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="5fbf5-107">Pada menu fly-out di sebelah kanan, masuk ke **Pengaturan email > Balasan otomatis** (jika ini adalah kotak surat bersama, cukup klik **Balasan otomatis** pada fly-out).</span><span class="sxs-lookup"><span data-stu-id="5fbf5-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="5fbf5-108">**Metode 2**</span><span class="sxs-lookup"><span data-stu-id="5fbf5-108">**Method 2**</span></span>

1. <span data-ttu-id="5fbf5-109">Masuk ke portal admin Office 365 menggunakan kredensial administrator.</span><span class="sxs-lookup"><span data-stu-id="5fbf5-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="5fbf5-110">Perluas **Pusat Admin**, lalu klik **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="5fbf5-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="5fbf5-111">Klik gambar di sudut kanan atas, klik **Pengguna Lain**, lalu pilih kotak surat pengguna yang ingin Anda ubah.</span><span class="sxs-lookup"><span data-stu-id="5fbf5-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="5fbf5-112">Di sisi kiri, pilih **Opsi**, klik **Atur Email**, lalu klik **Balasan otomatis.**</span><span class="sxs-lookup"><span data-stu-id="5fbf5-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="5fbf5-113">**Metode 3**</span><span class="sxs-lookup"><span data-stu-id="5fbf5-113">**Method 3**</span></span>

<span data-ttu-id="5fbf5-114">Jalankan cmdlet berikut ini di Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5fbf5-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="5fbf5-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="5fbf5-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="5fbf5-116">Untuk informasi selengkapnya tentang cmdlet ini, lihat [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="5fbf5-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
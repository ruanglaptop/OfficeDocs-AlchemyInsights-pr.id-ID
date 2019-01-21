---
title: Memindahkan pesan email ke kotak pesan arsip
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295566"
---
Mengalami masalah pengarsipan item ke kotak pesan arsip. Pastikan Anda telah melakukan langkah-langkah berikut:
  
1. Mengkonfirmasi bahwa **arsip pesan** telah diaktifkan. Jika tidak, gunakan langkah-langkah dalam [artikel ini](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) untuk mengaktifkan kotak pesan arsip. 
    
2. Di pusat Admin Exchange, pilih **Tag penyimpanan** di bawah **Manajemen kepatuhan**, membuat **tag penyimpanan** dengan tindakan **Pindahkan ke arsip** yang mengandung diinginkan **Waktu penyimpanan**.
    
3. Di pusat Admin Exchange, pilih **Kebijakan penyimpanan**, membuat **Kebijakan penyimpanan** dan menambahkan Anda **Pindahkan ke arsip** tag penyimpanan ke kebijakan itu. 
    
4. [Menetapkan kebijakan penyimpanan](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) untuk kotak pesan pengguna tertentu. Kebijakan yang sama akan diterapkan ke **utama** dan kotak pesan **Arsip** . 
    
Kotak pesan pengguna sekarang harus memiliki kebijakan pengarsipan untuk memindahkan item ke kotak pesan arsip. Mungkin perlu untuk memaksa berhasil Folder asisten (MFA) untuk menjalankan dan menerapkan pengaturan baru untuk kotak pesan pengguna. Jalankan perintah berikut saat [terhubung ke EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) agar Bantuan Folder yang dikelola untuk kotak pesan tertentu: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Ingin informasi lebih lanjut tentang pengaturan kebijakan pengarsipan, lihat [menetapkan kebijakan kotak pesan arsip dan penghapusan](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

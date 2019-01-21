---
title: Memecahkan masalah sinkronisasi sandi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295235"
---
# <a name="troubleshoot-password-synchronization"></a>Memecahkan masalah sinkronisasi sandi

Untuk mengatasi masalah yang mana tidak ada password disinkronisasi dengan Azure iklan menghubungkan versi 1.1.614.0 atau yang lebih baru:
  
1. Buka sesi Windows PowerShell yang baru pada server Azure iklan menghubungkan Anda dengan pilihan **Jalankan sebagai Administrator** . 
    
2. Menjalankan **Set-executionpolicy tidak RemoteSigned** atau **tak Set-executionpolicy tidak dibatasi**. 
    
3. Mulai wizard Azure iklan terhubung.
    
4. Menavigasi ke ** tambahan tugas ** halaman, pilih ** mengatasi masalah **, lalu klik **berikutnya**. 
    
5. Pada halaman Troubleshooting, klik menu **peluncuran untuk mulai mengatasi masalah** di PowerShell. 
    
6. Di menu utama, pilih **Memecahkan sandi sinkronisasi**. 
    
7. Dalam sub menu, pilih **sinkronisasi Password tidak bekerja sama sekali**. 
    
 **Memahami hasil tugas pemecahan masalah**
  
Pemecahan masalah tugas melakukan pemeriksaan yang berikut:
  
- Memvalidasi bahwa fitur sinkronisasi password diaktifkan untuk penyewa Azure iklan Anda.
    
- Memvalidasi bahwa server Azure iklan terhubung tidak berada di pementasan mode.
    
- Untuk setiap ada lokal Active Directory connector (yang berhubungan dengan forest Active Directory yang ada):
    
- 
  - Memvalidasi bahwa fitur sinkronisasi password diaktifkan.
    
  - Pencarian untuk sandi sinkronisasi detak jantung peristiwa di log peristiwa Windows aplikasi.
    
  - Untuk setiap domain Active Directory di bawah konektor Active Directory lokal:
    
  - Memvalidasi bahwa domain dapat dicapai dari server Azure iklan terhubung.
    
  - Memvalidasi bahwa account Active Directory Domain Services (AD DS) yang digunakan oleh konektor Active Directory lokal memiliki benar username, password, dan izin yang diperlukan untuk sinkronisasi password.
    
Untuk bantuan lebih lanjut pemecahan masalah sinkronisasi sandi, lihat [mengatasi masalah sinkronisasi password dengan Azure iklan menyambung sinkronisasi](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

---
layout: post
en-title: Solving the Too-Many-Web-Servers Problem
id-title: Solusi untuk Masalah Terlalu Banyak Web Server
tags: productivity
permalink: too-many-web-servers
en-desc: How I built a lightweight internal portal to manage dozens of production and pre-production web servers.
id-desc: Bagaimana saya membangun portal internal ringan untuk mengelola puluhan web server produksi dan pra-produksi.
featured: true
---

<div style="text-align: justify;" data-lang="en">
  <p>When I first joined my company, one of the biggest headaches I faced wasn't the work itself—it was just trying to figure out <em>where everything was</em>. We had a <strong>ton of web servers</strong>. Some were for <strong>production</strong>, others were for <strong>pre-production</strong>, and each had its own quirks. On top of that, different systems required different levels of access—some were admin-only, others for testers or developers. To make it more complicated, the URLs were scattered across internal docs, chat messages, and the occasional browser bookmark. It was chaos.</p>

  <p>At first, I tried using bookmarks to organize the mess, but it quickly became clear that wasn’t enough. Bookmarks rely on the browser environment—some of our internal servers only work with specific secure browsers. If I opened the wrong link in the wrong browser, I’d either get an error or worse, be told the session couldn’t even start. It just didn’t scale. The friction was constant, and frankly, it made onboarding painful.</p>

  <p>And so, I decided to build something better. I created a <strong>unified web access portal</strong>, completely written in <strong>plain HTML and CSS</strong>—nothing fancy, just solid and simple. Think of it like a dashboard, but inspired by the minimalist aesthetic of <strong>imageboards like 4chan</strong>. I liked the idea of separating things visually and conceptually by <strong>app and operation type</strong>, just like how threads are broken up by topic.</p>

  <img src="assets/img/e5284689a95bd5a0c2bcb7367de7a8673a7a55b122586a0539d4dfb8fa90dcdf.webp" alt="4chan Boards">

  <p>Instead of searching through bookmarks or wikis, I could now go to a single page, click the relevant app group—say, "Payment Service – Prod" or "User API – Preprod"—and go directly to the login page, knowing it was the right environment and that my browser was compatible. I even tagged which environments required certain access roles, like admin or test accounts. The design was intentionally <strong>low-stimulation and functional</strong>, which helped me focus.</p>

  <img src="assets/img/68ad767d3e44ed77005f52e43af97c72d8f173d6f0fc193d84541c1a018dc1ea.webp" alt="Board">

  <p>I’ll be honest: this also played to how my brain works. As much as I hate to admit it, <strong>I’m not a great multitasker</strong>—and science has some backing that male brains in general aren’t naturally wired for heavy multitasking. The more cognitive overhead I could offload, the better. I didn’t want to have to <em>remember</em> server names, environments, access rules, or which browser to use. I just wanted to do my work.</p>

  <p>This portal turned into one of the most helpful tools in my daily workflow. What started as a personal hack became something teammates began asking for. Now, we’re considering making it part of our onboarding process. It’s lightweight, secure (since it’s just local static HTML), and surprisingly effective.</p>
                <img src="assets/img/96f5fc85bc9db329806237b8fb1831341f9c212217887de269fc65d535cd5e00.webp" alt="Board">
  <p>No frameworks, no JavaScript, no servers. Just <strong>HTML, CSS</strong>, and a little inspiration from imageboard culture.</p>

  <p>Sometimes, the best solutions are the ones that strip things down to the essentials.</p>
</div>

<div style="text-align: justify;" data-lang="id" class="hidden">
  <p>Ketika saya pertama kali bergabung dengan perusahaan saya, salah satu hal paling membuat pusing yang saya hadapi
    bukanlah pekerjaannya sendiri—melainkan hanya mencoba mencari tahu <em>di mana semua hal berada</em>. Kami memiliki
    <strong>banyak sekali server web</strong>. Beberapa untuk <strong>produksi</strong>, lainnya untuk
    <strong>pra-produksi</strong>, dan masing-masing punya keunikan sendiri. Di atas itu semua, sistem yang berbeda
    memerlukan tingkat akses yang berbeda pula—ada yang hanya untuk admin, ada yang untuk tester atau developer. Yang
    membuat makin rumit, URL-URL tersebar di berbagai dokumen internal, pesan chat, dan kadang-kadang di bookmark
    browser. Sungguh kacau.</p>
  <p>Pada awalnya, saya mencoba menggunakan bookmark untuk mengatur semuanya, tetapi dengan cepat saya sadar itu tidak
    cukup. Bookmark bergantung pada lingkungan browser—beberapa server internal kami hanya bisa diakses melalui browser
    aman tertentu. Jika saya membuka tautan yang salah di browser yang salah, saya bisa mendapat error atau bahkan lebih
    parah lagi, sesi tidak bisa dimulai sama sekali. Itu tidak bisa diandalkan. Gesekan terus-menerus, dan sejujurnya,
    membuat proses onboarding sangat menyulitkan.</p>
  <p>Jadi, saya memutuskan untuk membangun sesuatu yang lebih baik. Saya membuat sebuah <strong>portal akses web
      terpadu</strong>, sepenuhnya ditulis dalam <strong>HTML dan CSS polos</strong>—tidak ada yang mewah, hanya
    sederhana dan solid. Bayangkan seperti dashboard, tetapi terinspirasi dari estetika minimalis <strong>imageboard
      seperti 4chan</strong>. Saya suka ide memisahkan hal-hal secara visual dan konseptual berdasarkan <strong>aplikasi
      dan tipe operasi</strong>, persis seperti bagaimana thread dipecah berdasarkan topik.</p> <img
    src="assets/img/e5284689a95bd5a0c2bcb7367de7a8673a7a55b122586a0539d4dfb8fa90dcdf.webp" alt="4chan Boards">
  <p>Alih-alih mencari di antara bookmark atau wiki, sekarang saya cukup membuka satu halaman, klik grup aplikasi yang
    relevan—misalnya, "Layanan Pembayaran – Prod" atau "User API – Preprod"—dan langsung menuju halaman login, dengan
    keyakinan bahwa itu adalah lingkungan yang benar dan browser saya kompatibel. Saya bahkan menandai lingkungan mana
    yang membutuhkan peran akses tertentu, seperti akun admin atau testing. Desainnya sengaja dibuat <strong>minim
      rangsangan dan fungsional</strong>, yang membantu saya tetap fokus.</p>
        <img src="assets/img/68ad767d3e44ed77005f52e43af97c72d8f173d6f0fc193d84541c1a018dc1ea.webp" alt="Board">
  <p>Sejujurnya, ini juga sesuai dengan cara kerja otak saya. Meski enggan mengakuinya, <strong>saya bukan seorang
      multitasker yang hebat</strong>—dan sains mendukung bahwa otak pria pada umumnya memang tidak dirancang secara
    alami untuk multitasking berat. Semakin banyak beban kognitif yang bisa saya hilangkan, semakin baik. Saya tidak mau
    <em>mengingat</em> nama server, lingkungan, aturan akses, atau browser mana yang harus digunakan. Saya hanya ingin
    menyelesaikan pekerjaan saya.</p>

  <p>Portal ini berubah menjadi salah satu alat paling membantu dalam alur kerja harian saya. Apa yang awalnya merupakan
    solusi pribadi, kini menjadi sesuatu yang mulai diminta oleh rekan-rekan kerja. Sekarang, kami sedang
    mempertimbangkan untuk menjadikannya bagian dari proses onboarding. Ini ringan, aman (karena hanya HTML statis
    lokal), dan sangat efektif.</p>
                    <img src="assets/img/96f5fc85bc9db329806237b8fb1831341f9c212217887de269fc65d535cd5e00.webp" alt="Board">
  <p>Tidak ada framework, tidak ada JavaScript, tidak ada server. Hanya <strong>HTML, CSS</strong>, dan sedikit
    inspirasi dari budaya imageboard.</p>

  <p>Terkadang, solusi terbaik adalah yang merangkum segala hal ke dalam bentuk paling esensial.</p>
</div>
---
layout: post
en-title: How I Turned Kakeibo Budgeting Simpler
id-title: Menyederhanakan Anggaran Kakeibo
tags: self-improvement productivity
permalink: kakeibo-telegram-bot
en-desc: From reading a traditional Japanese budgeting book to building a digital companion that fits in my pocket.
id-desc: Dari membaca buku anggaran tradisional Jepang hingga membangun pendamping digital yang bisa dibawa ke mana-mana.
featured: true
---

<div style="text-align: justify;" data-lang="en">
  <p>Last week, I read a book on personal finance called <em>Kakeibo</em> — the traditional Japanese method of mindful budgeting. It’s a simple, elegant system designed to make you think before spending, reflect regularly, and build a stronger relationship with your money. The approach emphasizes intention and awareness over complex tools, and it resonated with me immediately.</p>

  <p>But there was one major drawback: it was all on paper. Kakeibo encourages you to carry a notebook, record expenses manually, reflect weekly and monthly, and write down your financial goals. While beautiful in theory, the physical format quickly became inconvenient in daily life — especially for someone constantly on the move and already managing most tasks digitally.</p>

  <p>That’s when I had the idea: what if I could build a Telegram bot to help me follow the Kakeibo method in a more practical, accessible way? I already use Telegram every day — it’s fast, always with me, and supports bots well. I didn’t want a full-fledged budgeting app with graphs and dashboards. I wanted a simple, minimal tool that asked the right questions and supported the reflective process without adding complexity.</p>

<img src="assets/img/95436eae6b567491e0ed495d593d185db0e429c33363a1d5d3d6bed6944e1359.webp" alt="Feature">

  <p>To build the bot, I chose <strong>Go</strong> as the main backbone for handling Telegram interactions. Go is fast, efficient, and once compiled, it's incredibly easy to deploy across different environments. <span style="background-color: rgb(173, 255, 195);">I liked the idea of having a single binary that just runs without the need for a complex runtime or virtual environment.</span> It made the bot reliable and portable — perfect for a small, personal project like this.</p>

  <p>For data storage, I used <strong>SQLite</strong>. <span style="background-color: rgb(173, 255, 195);">Since this bot is primarily for my own use, I didn’t need a full-blown server-based database like MySQL or PostgreSQL.</span> SQLite is lightweight, file-based, and requires zero setup. It integrates cleanly with Go, and it handles the task of storing expenses, categories, and summaries without any hassle.</p>

  <img src="assets/img/2a353f5ffc3a912460e2328d017e3f85997bd82d7d596419c01f009136b7c3cd.webp" alt="Project Structure">

  <p>To process the data and generate reports, I leaned on <strong>Python</strong>. It’s my go-to tool when it comes to data manipulation, exporting to Excel, or visualizing summaries.<span style="background-color: rgb(173, 255, 195);"> I wrote a few Python scripts that read the SQLite data and output weekly or monthly reports. This separation between the bot logic in Go and the reporting logic in Python kept the code modular</span>, and made it easy to iterate on each part independently.</p>
</div>

<div style="text-align: justify;" data-lang="id" class="hidden">
  <p>Minggu lalu, saya membaca sebuah buku tentang keuangan pribadi berjudul <em>Kakeibo</em> — metode tradisional Jepang untuk mengatur anggaran dengan penuh kesadaran. Ini adalah sistem yang sederhana dan elegan, dirancang untuk membuat Anda berpikir sebelum membelanjakan uang, melakukan refleksi secara rutin, dan membangun hubungan yang lebih kuat dengan uang Anda. Pendekatan ini menekankan niat dan kesadaran, bukan alat yang rumit, dan langsung terasa cocok bagi saya.</p>

  <p>Tapi ada satu kekurangan besar: semuanya berbasis kertas. Kakeibo mendorong Anda untuk membawa buku catatan, mencatat pengeluaran secara manual, melakukan refleksi mingguan dan bulanan, serta menuliskan tujuan keuangan. Meskipun indah secara teori, format fisik ini cepat terasa merepotkan dalam kehidupan sehari-hari — terutama bagi seseorang yang sering berpindah-pindah dan sudah mengelola sebagian besar tugas secara digital.</p>

  <p>Saat itulah saya mendapat ide: bagaimana kalau saya membangun sebuah bot Telegram untuk membantu saya menjalankan metode Kakeibo dengan cara yang lebih praktis dan mudah diakses? Saya sudah menggunakan Telegram setiap hari — cepat, selalu tersedia, dan mendukung bot dengan baik. Saya tidak menginginkan aplikasi pengatur anggaran penuh dengan grafik dan dasbor. Saya hanya ingin alat yang sederhana dan minimalis yang mengajukan pertanyaan yang tepat dan mendukung proses refleksi tanpa menambah kerumitan.</p>

  <img src="assets/img/95436eae6b567491e0ed495d593d185db0e429c33363a1d5d3d6bed6944e1359.webp" alt="Feature">

  <p>Untuk membangun bot-nya, saya memilih <strong>Go</strong> sebagai tulang punggung utama dalam menangani interaksi dengan Telegram. Go cepat, efisien, dan setelah dikompilasi, sangat mudah dijalankan di berbagai lingkungan.<span style="background-color: rgb(173, 255, 195);"> Saya menyukai gagasan memiliki satu file biner yang langsung bisa dijalankan tanpa runtime atau lingkungan virtual yang rumit.</span> Ini membuat bot menjadi andal dan portabel — sempurna untuk proyek kecil dan pribadi seperti ini.</p>

  <p>Untuk penyimpanan data, saya menggunakan <strong>SQLite</strong>. <span style="background-color: rgb(173, 255, 195);">Karena bot ini terutama digunakan untuk keperluan pribadi, saya tidak memerlukan database server seperti MySQL atau PostgreSQL.</span> SQLite ringan, berbasis file, dan tidak memerlukan pengaturan apa pun. SQLite terintegrasi dengan baik dengan Go, dan mampu menangani penyimpanan pengeluaran, kategori, serta ringkasan dengan mudah.</p>

<img src="assets/img/2a353f5ffc3a912460e2328d017e3f85997bd82d7d596419c01f009136b7c3cd.webp" alt="Project Structure">

  <p>Untuk memproses data dan menghasilkan laporan, saya menggunakan <strong>Python</strong>. Ini adalah alat andalan saya untuk manipulasi data, ekspor ke Excel, atau visualisasi ringkasan. <span style="background-color: rgb(173, 255, 195);">Saya menulis beberapa skrip Python yang membaca data dari SQLite dan menghasilkan laporan mingguan atau bulanan. Pemisahan antara logika bot di Go dan logika pelaporan di Python membuat kode menjadi modular</span>, dan memudahkan pengembangan setiap bagian secara terpisah.</p>
</div>


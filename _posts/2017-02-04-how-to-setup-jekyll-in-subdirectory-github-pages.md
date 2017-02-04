---
layout: post
title: How to setup jekyll in subdirectory in github pages
published: true
date: '2017-02-04'
tags:
  - tutorial
---
Sebelum bikin blog menggunakan jekyll pada github pages ini, sebelumnya saya sudah pernah buat github static page (without jekyll, only using html js and css). Jadi karena sudah terlanjut punya static page yang saya gunakan untuk portofolio online yang bisa di akses [disini](https://sukorenomw.github.io). Rasanya sayang untuk bikin github page ini jadi full jekyll (belum lagi mikirin bagaimana mindahin portfolio yang sudah ada ini ke format jekyll).

Lalu yang saya inginkan itu nambah blog pada github page yang sudah ada itu, tanpa harus mengubah portofolio yang hanya html css dan js ke format jekyll. caranya bagaimana ? saya terpikir untuk buat blog menjadi page baru yaitu [https://sukorenomw.github.io/blog](https://sukorenomw.github.io/blog).

## Prologue

awalnya saya coba buat folder baru di repository yang sudah ada, bernama blog, lalu saya setup jekyll disana (banyak sekali tutorial setup jekyll di github page, salah satunya [ini](https://jekyllrb.com/docs/github-pages/)). ternyata cara yang ini gagal, tidak semudah yang di bayangkan.

Lalu sempat cari-cari tutorial di google, ada beberapa tutorial, tapi hampir semua nya tidak jelas, mungkin susah di baca bagi orang awam yang baru pertama kali setup jekyll, akhirnya saya menemukan yang agak jelas (walaupun masih belum jelas untuk seorang awam) yaitu blog dari [Eamonn Bell](http://www.eamonnbell.com/blog/2014/08/21/github-pages-subdirectory-hassle/), dan akhirnya setelah baca-baca darisana, saya berhasil juga bikin blog ini dan akhirnya saya putuskan untuk membuat cara setup step-by-step yang lebih jelas, sekaligus dokumentasi apa yang saya lakukan.

## How to setup jekyll in subdirectory

1. langkah pertama yang perlu dilakukan adalah, membuat repository baru di [github](https://github.com), karena saya mau buat blog dengan link baru : [/blog](https://sukorenomw.github.io/blog), maka saya buat repository bernama blog.

2. setup jekyll pada repository tersebut, saya anggap pembaca sudah bisa setup jekyll, jika belum silahkan scroll ke atas.

3. yang ~~paling~~ penting adalah, untuk membuat subdirectory pada github page, kita harus membuat branch bernama **gh-pages**, jadi semua commit harus masuk ke branch ini, bukan branch master

4. ternyata ini bagian paling penting, kita harus mengubah beberapa setting di **config.yml**

        baseurl: "/blog"
        production_url : http://<username>.github.io/blog

---
layout: post
published: false
title: 'Some hacking ? '
---
Setelah sekian lama belum nulis lagi, akhirnya ada niat untuk nulis, kali ini cuman akan ngelist beberapa hacking tools dan istilah hacking yang beberapa bulan ke belakang sedang saya explorasi. 

tulisan ini cuman akan ngelist tanpa masukin PoC penggunaannya, supaya ingat juga apa saja yang di explorasi, karena PoC masing-masing tools dan vulnerability akan saya bahas di post-post berikutnya (biar banyak artikelnya).

list-list yang baru-baru ini di eksplorasi sebenarnya bukan merupakan bug-bug atau vulnerability baru (kebanyakan old vuln) tetapi tetap saja masih banyak website-website yang masih "ngebug" terhadap vulnerability-vulnerability ini.

## Phising & Redirection
- [open redirect](https://www.owasp.org/index.php/Unvalidated_Redirects_and_Forwards_Cheat_Sheet)
- [reverse tabnabbing](https://danielstjules.github.io/blankshield/)

### Tools :
- bisa dilakukan tanpa menggunakan tools khusus

## MITM and Sniffing
- [Man-In-The-Middle](https://www.owasp.org/index.php/Man-in-the-middle_attack)

### Tools:
- [mitmproxy](https://mitmproxy.org/)
- [charles](https://www.charlesproxy.com)
- [Packet Capture](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture)

## Unauthorized Access
- [Repository Ripping](http://carnal0wnage.attackresearch.com/2015/03/devooops-revision-control-git.html)

### Tools:
- [dvcs-ripper](https://github.com/kost/dvcs-ripper)
- [Git Pawn](https://github.com/allyshka/pwngitmanager)

## Takeover
- [Subdomain takeover]()

### Tools:
- [knockpy](https://github.com/guelfoweb/knock)

## Reverse Engineering
- 
### Tools:
- [apktool](https://ibotpeaches.github.io/Apktool/)

Tools-tools yang saya tulis diatas, tidak sepenuhnya bisa membuat hacking menjadi sangat mudah, tetapi tools tersebut bisa memudahkan untuk mendapatkan informasi
---
layout: post
title:  "Masang Clojure."
date:   2016-02-12 07:11:25 +0700
description: "Masang dulu clojure lah di komputer kamu sebelum ngdoding clojure"
categories: clojure how-to
---

Kalau mau belajar Clojure, mesti punya Clojure dulu atuh yah di mesin kitanya. Masang Clojure di komputer kita itu lumayan gampang sih, karena ada yang namanya Leiningen. Nantinya si Leiningen bakal ngebantu kita masang Clojure di komputer kita. Terus tugas Leiningen juga buat ngatur hal-hal yang berhubungan/dibutuhkan sama projek(program) Clojure kita. Contoh: Kan biasanya projek kita tuh butuh kayak library atau plugin kayak gitu. Nah si Leiningen ini teh tugasnya buat kayak gitu, memastikan library/plugin yang kita butuhin tuh bisa dipake di projek kita. Kalau di Ruby mah ada kayak Gemfilenya gitu. Terus Leiningen juga dipake buat nentuin nama atau versioning atau lisensi projek Clojure kitanya. Kayak gitu-gitu.

Sebelum masang Leiningen, karena Clojure itu jalan diatas JVM(Java Virtual Machine), komputer kita mesti punya dulu JVM minimal versi 1.6 lah.  Masang JVM mah bisa kali ya. Kesini aja: [http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html) buat ngecek apa di mesin kita udah kepasang JVM, cek aja pake command ini di terminal atau CMD kamu:

{% highlight comandline %}
  java -version
{% endhighlight %}

Udah kepasang JVM, kita tinggal masang Leiningen. Coba cek [http://leiningen.org/](http://leiningen.org/) disana juga ada installer buat pengguna Windows juga. Iya, pengguna Windows juga bisa ngembangin pake Clojure juga kok tenang aja.
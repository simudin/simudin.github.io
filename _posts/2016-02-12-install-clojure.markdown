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
  $ java -version
{% endhighlight %}

Udah kepasang JVM, kita tinggal masang Leiningen. Coba cek [http://leiningen.org/](http://leiningen.org/) disana juga ada installer buat pengguna Windows juga. Iya, pengguna Windows juga bisa ngembangin pake Clojure juga kok tenang aja.

Oke sekarang saya cuma nunjukin cara install di Ubuntu, kalau buat di OSX atau di Windows coba google.

Download 'lein script' yang ada di halaman tersebut. terus save skrip tersebut jadi text biasa aja ga perlu pake extension. Udah dapet skripnya, simpen skripnya di path dimana shell kamu bisa ngeksekusi skrip tersebut.

Contoh, di direktori home(~) komputer kamu biasanya itu ada direktori namanya 'bin'. Simpen sana aja. Kalau ga ada direktori namanya 'bin', bikin dulu aja. Caranya:

Masuk dulu ke direktori home kamu pake perintah
{% highlight comandline %}
  $ cd ~
{% endhighlight %}

Terus, bikin direktori buat tempat eksekusi file yang bisa dieksekusi(executable).
{% highlight comandline %}
  $ mkdir bin
  $ echo "export PATH=$PATH:$HOME/bin" >> ~/.bashrc
{% endhighlight %}

Kenapa namanya harus 'bin'? Coba google. Nah, terus masukin skrip 'lein' yang tadi didownload ke direktori 'bin' yang udah dibikin.
{% highlight comandline %}
  $ cp tempat/file-lein/berada/lein ~/bin
{% endhighlight %}

Udah gitu, rubah file skrip 'lein' tersebut jadi file yang executable. caranya
{% highlight comandline %}
  $ chmod a+x ~/bin/lein
{% endhighlight %}

Kalau filenya udah berubah jadi file executable, tinggal jalanin pake
{% highlight comandline %}
  $ ~/bin/lein
{% endhighlight %}

Nanti si file tersebut bakalan otomatis ngedownload clojure buat komputer kita.

Kalau prosesnya udah berhasil tinggal cek pake perintah:
{% highlight comandline %}
  $ lein repl
{% endhighlight %}

Nanti bakalan muncul kira-kira kaya gini:
{% highlight comandline %}
  nREPL server started on port 33066 on host 127.0.0.1 - nrepl://127.0.0.1:33066
  REPL-y 0.3.7, nREPL 0.2.12
  Clojure 1.8.0
  Java HotSpot(TM) Server VM 1.8.0_72-b15
      Docs: (doc function-name-here)
            (find-doc "part-of-name-here")
    Source: (source function-name-here)
   Javadoc: (javadoc java-object-or-class-here)
      Exit: Control+D or (exit) or (quit)
   Results: Stored in vars *1, *2, *3, an exception in *e

  user.core=>
{% endhighlight %}

Kalau udah muncul kaya gitu. Berarti itu Clojure udah kepasang di komputer kita. 

Gitu. Nanti di postingan berikutnya kita lanjut kenalan sama sintak clojure. 

Dah!
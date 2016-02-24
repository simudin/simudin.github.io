---
layout: post
title:  "Bentuk sintak Clojure."
date:   2016-02-12 07:11:25 +0700
description: "Bentuk sintak clojure."
categories: clojure
---

Baiklah, sekarang mari kita bahas bentuk sintak dari Clojure. 

Karena Clojure ini salah satu "*dialect*" dari Lisp. Maka sintak clojure ini banyak banget pake kurung buka/kurung tutup (*parenthesis*). Yang begini `(` sama yang `)`. Masuk dulu ke REPL Clojure buat nyoba nulis sintak clojure. Caranya masuk REPL, pastikan kamu udah install dulu clojure pake leiningen, terus buka terminal atau command line di komputer kamu, terus ketik:
{% highlight comandline %}
$ lein repl
{% endhighlight %}

`$` nya ga usah ikutan diketik, itu cuma tanda aja bahwa kamu sedang berada di prompt terminal/CMD.

Kalau Clojurenya udah ke install nanti bakal muncul:
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

user=>
{% endhighlight %}

Lihat baris paling akhir yang `user=>`. Nah di baris itu kita bisa nulis kode sintaknya.

### **REPL itu apa ya?**

REPL itu singkatan dari *Read Eval Print Loop*. REPL itu alat yang berguna banget buat nyoba kode langsung tanpa harus ngesave dulu kodenya di file terus di compile buat tau hasil dari kode kita. Ga usah! Kalau pake REPL, kita tinggal tulis langsung kode kita di promptnya terus tekan `ENTER`deh buat tau hasilnya. REPL ga cuma ada di Clojure sih, di bahasa pemrograman lain juga ada tapi ga banyak. Yang saya tau REPL itu ada juga di Ruby sama Python.

Mari kita coba biar tau bagaimana REPL bekerja. Ketik di prompt REPL kamu:
{% highlight comandline %}
user=> (+ 1 2)
{% endhighlight %}

`user=>` nya ga usah ikutan diketik, itu cuma tanda aja bahwa kamu sedang berada di prompt REPL.

Kalau udah ditulis `(+ 1 2)` terus tekan `ENTER`. Nanti bakal muncul kayak gini:
{% highlight comandline %}
user=> (+ 1 2)
3
user=> 
{% endhighlight %}
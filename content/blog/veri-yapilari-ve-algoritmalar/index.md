---
title: "Veri Yapıları Ve Algoritmalar"
date: 2022-02-18T23:56:26+03:00
categories: ['Yazılım']
tags: ['veri yapıları','algoritmalar','linked list']
description: ""
draft: true
---
{{<figure src="veri_yapilari_ve_algoritmalar.png">}}

**Veri yapıları** ve **Algoritmalar** konuları tek bir blog sayfasına sığmayacak kadar geniş bir konu. [Patika.dev](https://patika.dev) üzerinden takip ettiğim Java eğitimleri kapsamında aldığım veri yapıları derslerine ilişkin notlarımı paylaşmakta fayda görüyorum. Konuyu derinlemesine öğrenmek isteyenler için [şu](https://palmeyayinevi.com/algorItmalara-gIrIs) kitabı inceleyebilirler.

# 1-Veri Yapıları
> Veri yapısı, veriye erişimi ve üzerinde yapılacak değişiklikleri kolaylaştırmayı amaçlayan veri depolama ve düzenleme yöntemidir. Tüm amaçlar için geçerli tek bir veri yapısı yoktur, bu yüzden veri yapılarının bir çoğunun kabiliyet ve sınırlarını bilmek önemlidir.  
> (Algoritmalara Giriş - Palme Yayıncılık)

Burada 4 farklı veri yapsına değinmeye çalışacağım;
- Array
- Linked List
- Stack
- Queue
## 1.a. Array
{{<figure src="array.gif">}}
Aynı tip verilerin yan yana sıralandığı veri yapısıdır. Ne kadar veriye ihtiyaç duyuluyorsa hafızadan o kadar yer ayrılmaktadır (*dinamik olmayan dizilerde*)
Sabit dizilere, dizi tanımlanırken belirlenenden fazla veri eklemezken, dinamik dizilere sonradan da veri ekleme yapılabilmektedir. Fakat bu ekleme işlemi, mevcut dizinin tamamının hafızadan başka bir yere tekrar kopyalanması ile gerçekleşmektedir. Bu sebeple dizi boyutu büyüdükçe maliyetde artmaktadır.

{{< alert >}}
**AVANTAJ:** İstenilen veri oldukça hızlı bir şekilde bulunabilmektedir.  

**DEZAVANTAJ:** Kullanılmayacak olmasına rağmen hafızada fazla yer ayırmak gerekebilir. Ayrıca yeni bir veri eklenmek istendiğinde dizinin tamamı hafızada başka bir yere taşınmak zorunda kalabilir, bu durum maliyet oluşturmaktadır. Veri ekleme çıkarma işlemi, veri sayısı arttıkça maliyetli olur.
{{< /alert >}}

## 1.b. Linked List
{{<figure src="linkedlist.png">}}
Linked List'te her bir eleman tutması gereken veriyi ve kendisinden sonra gelen elamanın adresini tutar. Bu sayede, dizilerde olduğu gibi verilerin ardı ardına dizilme zorunluluğu yoktur. Hafızada farklı yerlere dağılabilirler.

{{< alert >}}
**AVANTAJ:** Hafıza efektif olarak kullanılabilir. Veri kolaylıkla eklenip çıkarılabilir. Veri eklerken tek yapılması gereken, bir önceki verinin işaret ettiği yerin adresini değiştirmektir.  

**DEZAVANTAJ:** İçerisinde veriyi bulmak, veri sayısı arttıkça zorlaşır. Çünkü her bir adresi tek tek dolaşmak gerekir.
{{< /alert >}}

## 1.c. Stack
{{<figure src="stack.png">}}
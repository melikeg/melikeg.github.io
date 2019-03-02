---
title: Temel Terminal Komutları
---

Merhaba! Size bu yazımda temel terminal komutlarını anlatacağım. Öncelikle terminal nedir ile başlayalım.
 
# **TERMİNAL NEDİR?**
 
Terminal, linux işletim sistemli bilgisayarlarda ve apple bilgisayarlarda yer alır. Windows işletim sistemli bilgisayarlarda ise komut satırı veya komut istemcisi olarak bilinir. Bilgisayar dünyasında fare işaretleyicilerinin ve grafik arayüzlerinin olmadığı zamanlarda kullanılıyordu. Eğer yazılımla uğraşıyorsanız komut satırına yakın olmanız yazılım geliştirirken size çok büyük avantaj sağlayacaktır.

# **TERMİNAL KOMUTLARI**
 
Terminal komutları metinsel ifadelerle kullanıcının ve bilgisayarın iletişime geçmesini sağlar. Yani aslında dosya oluşturma işlemini masaüstünde fare yardımıyla yapabileceğimiz gibi terminalde de oluşturabiliriz ya da silebiliriz.
 
## cd

Change Directory kelimesinin baş harflerinden gelir. Bulunduğumuz dizini değiştirmek için kullanırız. Mesela aşağıdaki örnekte cd ile önce Projects klasörüne sonra da ruby klasörüne girdik. "cd.." komutuyla da bir alt dizine inebilirsiniz.

<blockquote>
<p>melike@DESKTOP-K6C47S6:~$ cd Projects</p>
<p>melike@DESKTOP-K6C47S6:~/Projects$ cd ruby</p>
<p>melike@DESKTOP-K6C47S6:~/Projects/ruby$ cd ..</p>
<p>melike@DESKTOP-K6C47S6:~/Projects$</p>
</blockquote>


## ls veya dir

Directory ve list kelimelerinin kısaltmalarıdır. Bu komutlar bulunduğunuz klasör içindeki dosyaları listeler.

<blockquote>
<p>melike@DESKTOP-K6C47S6:~$ ls</p>
<p>Projects  melikeg.github.io  wewanted</p>
<p>melike@DESKTOP-K6C47S6:~$ dir</p>
<p>Projects  melikeg.github.io  wewanted</p>
</blockquote>


Aynı zamanda,

* "ls -a" komutu ile gizli dosyaları
* "ls -l" komutu ile ayrıntılarıyla birlikte
* "ls -R" komutu ile tüm alt klasörleri
* "ls -t" komutu ile zamana göre sıralanmış şekilde listeleyebilirsiniz.

## help

help komutunu tek başına kullandığınızda tüm komular hakkında bilgi alabilirsiniz. Örneğin, cd komutu hakkında bilgi almak için "help cd" yazabilirsiniz.

## pwd

Klasörün tam konumunu gösterir.

<blockquote>
<p>melike@DESKTOP-K6C47S6:~$ pwd</p>
<p>/home/melike</p>
</blockquote>


## del
del komutunu dosya silmek için kullanırız. Kullanımı **del dosya_adı** şeklindedir. Bulunduğunuz dosyanın içindeki tüm dosyaları silmek istiyorsanız **del *** komutunu kullanmalısınız.

## rmdir
rmdir komutunu klasör silmek için kullanılırız ama yalnız yazılınca içi boş olan klasörleri siler. İçi dolu klasöerleri silmek için **/S**  parametresi eklememiz gerekiyor.

**rmdir /S klasör_adı**

Ayrıca rm komutu ile hem dosya hem klasör silebiliriz. **rm** yazarak dosya **-r** parametresi ekleyerek de klasör silebiliriz.

**rm dosya_adı**

**rm -r klasör_adı**

## mkdir
Make Directory kelimelerinin kısaltılmış halidir. mkdir komutunu yeni dizin oluşturmak için kullanırız. Aşağıdaki örnekte klasör klasörünün içini ls ile listeledik, boştu. mkdir ile klasörün içine notlar adında bir klasör oluşturduk.

<blockquote>
<p>melike@DESKTOP-K6C47S6:~/dosya$ ls</p>
<p>melike@DESKTOP-K6C47S6:~/dosya$ mkdir notlar</p>
<p>melike@DESKTOP-K6C47S6:~/dosya$ ls</p>
<p>notlar</p>
</blockquote>

## echo
Input olarak girilen yazıyı gönderildiği parametrelerle birlikte gösterir.

<blockquote>
<p>melike@DESKTOP-K6C47S6:~$ echo "Merhaba"</p>
<p>Merhaba</p>
<p>melike@DESKTOP-K6C47S6:~$ echo $((9+5))</p>
<p>14</p>
<p>melike@DESKTOP-K6C47S6:~$ echo {1,2,3,4}veya</p>
<p>1veya 2veya 3veya 4veya</p>
</blockquote>


## shutdown
Bilgisayarı belli bir süre sonra kapatmak için kullanılır.

## exit
Terminalden çıkmak için kullanılır.

## ctrl^c
Çalışan terminal işlemini sonlandırır.

## clear
Terminal ekranını temizlemek için kullanılır. clear yerine **cls** de yazılabilir.
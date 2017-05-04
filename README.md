**CoffeeScript Language | TR**
===================



#### <i class="icon-folder-open"></i> **CoffeeScript Tarihçesi**
13 Aralık 2009'da **Jeremy Ashkenas** tarafından çıkarılmış bir dildir.  Coffeescript dili 24 Aralıkta, ilk etiketli ve belgelenmiş **0.1.0** sürümü ile kullanıma sunulmuştur. CoffeeScript, gitHub üzerinde **açık kaynak kodlu** olarak geliştirilen bu dile günde 300'den fazla destek geliyordu.

Ashkenas, **24 Aralık 2010**'da, projenin ilk kez ilan edildiği Hacker Haber'e 1.0.0 kararlı sürümünü açıkladı. Günümüzde son versiyon olarak **1.12.5**'i kullanır.

#### <i class="icon-folder-open"></i> **CoffeeScript Nedir?**


**CoffeeScript** , JavaScript'e derlenen bir dildir. CoffeeScript'e en basit anlamıyla sadece Javascript'tir diyebiliriz. CoffeeScript'te yazdığınız her kodu Javascript'te yazmış gibi olursunuz. Aralarındaki fark neredeyse yok denecek kadar azdır. Javascript'in parantezlerini girintileri çıkıntılarını yok ederek yazılan bu dile coffeescript deniyor. Genellikle syntax ı sade, kullanışlı ve çabuk öğrenilebilmesinden ötürü sıklıkla kullanılmaktadır. Özetle çok sade bir yazım şekli olduğu söylenir; örneğin javascriptte yazmış oldunuz bu kod:

```
var kare = function(x) {
  return x * x;
}
```
CoffeeScript'te böyledir

```
kare = (x) ->
  x * x
```
#### <i class="icon-folder-open"></i> **Tasarım Amaçları**

CoffeeScript'in güzel yanlarından birisi, yazabileceğiniz kod yoğunluğudur. Bu sebeple insanlar tarafından sıklıkla tercih edilir. Bu dil ile yazacağınız projeyi coffeescript ile salt bir halde/dille oluşturmak çok kolaydır.

Programlama dillerinin çoğalmasının nedenlerinden biri, dil tasarımında çelişen büyük düşünce farklılıklarıdır. Genel durumda, diller iletişim amaçlıdır. Bir programlama dilini yayacak olan insan topluluğu dili net bir dille çok iyi bir şekilde anlatmalıdırlar ve aynı zamanda semantiği net bir şekilde yorumlamaya çalışan derleyicilerin kullanması gerektiğini bilmelidirler.

Derleyici, ne yaptığını daha doğru bir şekilde belirleyebilir, daha iyi kod üretebilir. Sen yanlış yazsan da o sana doğrusunu gösterebilir. Kod ne kadar açık olursa, okuması da o kadar kolay olur.

Coffeescipt'in en büyük amaçlarından birisi ise olabildiğince sade ve akıcı bir dil olmaktır. Geliştiricinin okumakta güçlük çektiği kod bu geliştiriceye zevk vermez.

Coffeescript dili, JavaScript listeleri içermez, ancak diziler ve nesneler gibi temeller bulunmaktadır.

CoffeeScript'te kısaca daha iyi bir örnek, nesne ve işlevin kısaltmasıdır. JavaScript nesnelerini oluşturmak için oldukça basit bir sözdizimi içeriyor olması çok fazla güzellik sağlıyor. CofffeeScript köşeli ayraçları atlıyor olması çok sade bir dille kod yazmanıza olanak sağlıyor.


#### <i class="icon-folder-open"></i> **Hedef Kitlesi**

Bu dilin hedef kitlesi, aktif olarak javascript yazan veya javascript benzeri bir dil kullanmak isteyip, bu dil tercihini yazımı sade, öğrenmesi kolay olandan yana kullanan kişiler tarafından kullanılan bir dil olduğu için hedef kitlesi bu tarafa biraz daha kaymaktadır.

#### <i class="icon-folder-open"></i> **Kullanım Alanları**

Öncelikle kendimden örnek verecek olursam. Ben nodejs ve Ruby on Rails projelerimde hem uyumlu çalışması ve hemde bahsettiğim üzere basit ve sade syntax'ını sevdiğim için kullanıyorum. Bunun yanında bir rails projesi oluşturduğunuzda defaull olarak içinde assets klasörü içinde javascript klasöründe sonu .js.coffee bitecek şekilde oluşturuyor.
Genel olarak coffeescript'in kullanım alanları bu şekildedir
> **Nasıl Kurabilirim**

> - npm install --global coffee-script

#### <i class="icon-folder-open"></i> **Desteklediği Paradigmalar**

>- Multi-paradigm
>- prototype-based
>- functional
>- imperative
>- scripting


#### <i class="icon-folder-open"></i> **Aritmetik İşlem Notasyonu**

>- postfix

#### <i class="icon-folder-open"></i> **Bellek Yönetimi**


**Chaplin** mimarisinin çekirdeği, en uygun bellek yönetimidir. JavaScript uygulamalarında gereksiz veri toplama hakkında geniş bir tartışma olmamasına rağmen, önemli bir konudur. Ana bellek yönetimine yardımcı olmak için, Chaplin, her denetleyicinin, modelin, koleksiyonun ve görünümün kendi başına temizlenmesini sağlayan güçlü bir silme süreci boyunca Backbone’s Modeli uygun görülmüştür,
Olay işleme ve nesneler arasında referanslar oluşturur. Bir görünüm, model değişikliklerini dinlerse, o modelin dahili _callbacks listesindeki bir görünüm yöntemine bir referansı vardır. Görünüm yöntemleri, genellikle, View.aspx.bind, _.bind (), CoffeeScript'in benzeri kullanarak görünüm örneğine bağlıdır. Bir değişiklik işleyicisi görünüme bağlı olduğunda, DOM zaten ayrılmış olsa bile görünüm bellekte kalır. Çöp toplayıcı bu referans nedeniyle hafızasını boşaltamaz.
Chaplin'de, yeni bir denetleyici devralınır ve kullanıcı arabirimi değiştikten sonra geçerli denetleyicinin kullanımdan kaldırma yöntemi çağrılır:
Denetleyici, model / koleksiyonlarında atma yöntemini çağırır ve onlara olan referanslarını kaldırır.
İmha edildiğinde, her model tüm özelliklerini temizler ve ilişkili tüm görünümleri ortadan kaldırır.
Bir görünümün elden çıkarma yöntemi tüm DOM öğelerini ortadan kaldırır, Bu elden çıkarma işlemi oldukça karmaşıktır ve birçok nesne özel bir atma yöntemine ihtiyaç duymaktadır. Ancak Chaplin'in yapabileceği en az şey budur.

#### <i class="icon-folder-open"></i> **Değişken kapsamları**

>- lexically scope

Değişkenleri dış kapsamda tanımlamanız gerekir. örneğin

```
counter = null
init = ->
  counter = 0
inc = ->
  counter += 1
```
#### <i class="icon-folder-open"></i> **Tip Sistemi ve Tip Kontrolü**

Elle bellek yönetimi ile C benzeri bir sistem sunan CoffeeScript bir diyalektidir. Tip sistemi (güçlü) ve tip kontrolü (static type checking) 'dir

#### <i class="icon-folder-open"></i> **Hello World**

```
$ ->
  console.log("HELLO COFFEESCRİPT")

```
ya da
```
$ ->
  alert("HELLO COFFEESCRİPT")

```

**ASAL SAYI HESAPLAMA**

```
text = ''
sayi = 0

asalHesapla = ->
  sayac = 0
  sayi = document.getElementById('sayi1').value
  i = 2
  while i < sayi
    if sayi % i == 0
      sayac++
    i++
  if sayac == 0
    text = 'Asal'
  else
    text = 'Asal değil.<br/> 1 ve Kendisi hariç <strong>' + sayac + '</strong> adet böleni var'
  document.getElementById('demo').innerHTML = text
  return
```

**FİBONACCİ HESAPLAMA**

```
i = undefined
fib = []
fib[0] = 0
fib[1] = 1
i = 2
while i <= 10
  # Next fibonacci number = previous + one before previous
  # Translated to JavaScript:
  fib[i] = fib[i - 2] + fib[i - 1]
  console.log fib[i]
  i++
```

**İKİLİ ARAMA (BİNARY SEARCH)**

```
binary_search = (val, L) ->
  return false if L.length == 0
  mid = Math.floor(L.length / 2)
  if L[mid] == val
    return mid
  else if val > L[mid]
    binary_search(val, L[(mid + 1)..(L.length)])
  else
    binary_search(val, L[0..(mid - 1)])

list = [1,2,3,4,5,6,7,8]
alert binary_search(18, list) # false
alert binary_search(3, list)  # 2
alert binary_search(6, list)  # 5
```
**SEZAR ŞİFRELEME**

```

caesarShift = (str, amount) ->

	# Wrap the amount
	if amount < 0
		return caesarShift(str, amount + 26)

	# Make an output variable
	output = '';

	# Go through each character
	for c, i in str

		# Get the character we'll be appending
		c = str[i]

		# If it's a letter...
		if c.match(/[a-z]/i)

			# Get its code
			code = str.charCodeAt(i)

			# Uppercase letters
			if (65 <= code <= 90)
				c = String.fromCharCode(((code - 65 + amount) % 26) + 65)

			# Lowercase letters
			else if (97 <= code <= 122)
				c = String.fromCharCode(((code - 97 + amount) % 26) + 97)

		# Append
		output += c

	# All done!
	output
```

**ERDEM OFLAZ** |
**BİLGİSAYAR MÜHENDİSLİĞİ** |
**14253046**

**KAYNAK**

http://stackoverflow.com

https://tr.wikipedia.org/wiki/CoffeeScript

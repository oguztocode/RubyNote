
# RubyNote
**RUBYYYY**

***[DEĞİŞKEN ATAMASI](https://www.educative.io/courses/learn-ruby-from-scratch/YQyokW33ky9)***

Ruby’de atama operatörünü kullanarak bir nesneye ad verebilirsiniz.

number = 1        “=” Atama Operatörü

puts number ⇒ 1 

***[DEĞİŞKEN ADLARINI YENİDEN KULLANMA](https://www.educative.io/courses/learn-ruby-from-scratch/gxMyAOy8qLj)***

number = 4

number = number * 3

puts number + 2 ⇒ 14 “Bu ifade ile aynı sonucu verir. puts 4 * 3 + 2  ⇒ 14

Kod Brifingi
Bir de mikroskop altında inceleyelim:

İlk satırda Ruby, sayıyı (nesneyi) oluşturur .
Daha sonra bu nesneye adıyla atıfta bulunmaya başlar number.
İkinci satırda , Ruby önce sağ taraftaki maddelere bakar ve ifadeyi değerlendirir number * 3.
Bunu yapmak için, sayıyı (nesneyi) yaratacak ve onu şu anda isme sahip olan nesne ile (number)çarpacaktır.
Bu işlem yeni bir number (nesne) ile sonuçlanır 12.
Şimdi Ruby nihayet adı number sonuca yapıştırmaya hazır, (12) yani bundan sonra isim numberfarklı bir nesneye atıfta bulunuyor, yani 12.
Üçüncü satırda Ruby, yine ilk number + 2 olarak sağdaki ifadeye bakacaktır.
Nesneyi yaratır (2) ve onu şu anda ada sahip olan nesneye ekler number.
Bu, yeni bir sayı (nesne) ile sonuçlanır 14.
Sonunda Ruby bu nesneyi (14) ekrana verir ve bu nesneyi (puts) ekrana verir.

**[SAĞDAKİ İFADELER İLK BAŞLAR.](https://www.educative.io/courses/learn-ruby-from-scratch/gxZ1W6AXNVj)**

number = 2 + 3 * 4 

puts number ⇒ 14

Ruby ilk satıra baktığında number = 2 + 3 * 4 bunun atama operatörünü kullandığını fark eder =.
Dolayısıyla sağdaki “şey”e (nesneye) isim atamadan önce o şeyin ne olduğunu bilmesi gerekir.

**Ruby Bunu Nasıl Yapıyor? #**
Yani, başka bir şey yapmadan önce, Ruby önce ifadeye bakacak 2 + 3 * 4 ve onu değerlendirecek, bu da sayı (nesne) ile sonuçlanacaktır 14.
Daha sonra bu nesneye adıyla atıfta bulunacaktır number(yani atama operatörünü değerlendirin =).
Ruby atamayı değerlendirmeye başladığında şu anda = kodun geçici olarak şöyle göründüğünü hayal edebilirsiniz number = 14 

(çünkü hesaplama sayıyı döndürmüştür).

2 Tane Ufak Soruyla Bu Bölümü Taçlandıralım Mı?

```ruby
	x = 12 - 2 + 4                  number = 3                   
	puts x                          number = 4
	Çıktı nedir?                    puts number 
  Cevap = 14                      number = 5 
                                  Çıktı nedir? 
																	Cevap = 5                                                                                                              
```

***[SAYILARLA ÇALIŞMAK](https://www.educative.io/courses/learn-ruby-from-scratch/q28kkmO3Q5k)***

Basitçe yazarak bir sayı oluşturabilirsiniz 123 Ruby kodudur ve 123 sayısını temsil eder. Ondalık olarak da noktalı bir biçimde de yazabilirsiniz (12.34).

Negatif sayılar bir eksi eklenerek oluşturulur (-99).

Büyük sayılarla çalışırken okunabilirliği arttırmak için “_” de kullanabilirsiniz.

100_000_00.23 sayısı tam olarak aynıdır bu sayı ile 10000000.23. Ancak bu kullanım kesinlikle isteğe bağlıdır.

**Sayı Çeşitleri**

Kaputun altında, çoğunlukla teknik nedenlerden dolayı, aslında farklı türde sayılar vardır ve bu türlerin her birinin başka alt türleri olabilir.

![Working with Numbers - Learn Ruby from Scratch - Google Chrome 19.03.2022 21_06_12.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/876a6807-5121-44a7-bd07-4cb8fb517c89/Working_with_Numbers_-_Learn_Ruby_from_Scratch_-_Google_Chrome_19.03.2022_21_06_12.png)

Integer “Tam Sayılar” Float “Ondalık Sayılar”

İlgili sayılarda birisi Float ise geri dönüş olarak Float alırız.

```ruby
puts 1.0 + 2           Çıktı 3.0
puts 1 + 2.0                 3.0
```

Bu bir bölme yaptığımızda önemlidir:

```ruby
puts 5 / 2.0                 Çıktı 2.5
puts 5 / 2                         2
puts 5.0 / 2                       2.5     
```

Bölme yaparken “Float” sayıları kullanmamız tavsiye edilir.

**SAYILARLA OYNAMAK**

```ruby
def play_with_numbers (hours_in-december, minute_in_december)
hours_in_december = 31 * 24
minutes_in_december = hours_in_december * 60
```

[**MODULO BULMA**](https://www.educative.io/courses/learn-ruby-from-scratch/gxMGRRN5qN9)

=Modulo Operatörü=

Ruby'de ”%” sembol modulo operatörünü temsil eder. İki pozitif sayının modulo'su, ilk sayıyı ikinci sayıya bölerseniz elde ettiğiniz kalandır. Örneğin (25 % 2) size vermeli (1).

Modulo operatörü, bir sayının başka bir sayıya bölünüp bölünemeyeceğini anlamak için süper kullanışlıdır çünkü sıfırdan kalanını görmeyi bekleriz.

```ruby
def calculate_mod(num1, num2)
result = num1 % num2
return result
end
```

***[TEK Mİ ÇİFT Mİ?](https://www.educative.io/courses/learn-ruby-from-scratch/N7YJwM7B1np)***

Bir tamsayı verildiğinde, o sayının çift olup olmadığını bulmanız gerekir. Eğer sayı çift ise geri dönmeniz gerekir ”0”, aksi takdirde geri dönün ”1”.

```ruby
def even_or_odd(num)
result num % 2 
return result 
end
```

***[STRİNGLERLE ÇALIŞMAK](https://www.educative.io/courses/learn-ruby-from-scratch/NE0WxPDjB9p)***

Dizeler, herhangi bir metni tek veya çift tırnak içine alarak tanımlanabilir.

***Dizilerle Yapabileceğimiz Şeyler***

```ruby
puts "snow" + " ball" => snowball
puts "hi" + "hi"+ "hi" => hihihi
puts "hi" * 3 => hihihi
puts "1" + "1" + "1" => 111
puts "1" * 3 => 111
```

```ruby
puts "hello".upcase
puts "hello".capitalize
puts "hello".length
puts "hello".reverse
puts "hello world".split("l")
```

```ruby
HELLO 
Hello
5
olleh
he o wor d
```

***[DİZE ENTERPOLASYONU](https://www.educative.io/courses/learn-ruby-from-scratch/RMPKNP3OpBw)***

Daha önce belirtildiği gibi + operatörünü kullanarak dizeleri birbiriyle birleştirebilirsiniz.

```ruby
name = "Ada"
puts "Hello, " + name + "!" => Hello, Ada!
```

İpleri bu şekilde birbirine yapıştırmak işe yarar ve bunu yapabilirsiniz. Bununla birlikte, aynısını gerçekleştirmenin başka bir yöntemi daha vardır ve yaygın olarak kullanılan ve genellikle (+).

```ruby
name = "Ada"
puts = "Hello, + #{name}!" => Hello, Ada!
```

Bu sözdizimini kullanarak, açılış **#{**ve kapanış **}**bitleri arasındaki her şey Ruby kodu olarak değerlendirilir ve bu değerlendirmenin sonucu onu çevreleyen dizeye *gömülür .*

Başka bir deyişle, Ruby **#{name}**bu dizgede bulduğunda, Ruby kodunun parçasını değerlendirecektir **name**. Bunun bir değişken olduğunu bulur, bu nedenle değişkenin dize olan değerini döndürür **"Ada"**. Böylece onu çevreleyen dizgeye gömerek yerine **"Hello, #{name}!"**koyar .**#{name}"Ada"**

Şimdi nihayet tek ve çift tırnak ile oluşturulan dizeler arasındaki farkı da açıklayabiliriz:

“Dşize enterpolasyonu yalnızca çift tırnak işareti ile çalışır.

Bu şu demek oluyor.

```ruby
puts "Interpolation works in double quoted strings: #{1 + 2}."
puts 'And it does not work in single quoted strings: #{1 + 2}.'
Interpolation works in double quoted strings: 3.
And it does not work in single quoted strings: #{1 + 2}.
```

Her şeyden önce, yine, yazmak için biraz daha az harf var. Örneğimizde, bu sadece beş karakter, önemli değil. Ancak, üç, dört veya daha fazla değişken kullanılarak oluşturulan daha uzun bir dize düşünün. Şimdi, bu fazladan boşluk hızla toplanır ve işler artık tek bir satıra sığmaz.

Örnek aşağıda size bir hata verecektir:

```ruby
puts "I am the number +3"
```

Ama bu gayet iyi yapacak:

```ruby
puts "I am the number #{3}" => I am the number 3
```

**NOT:**

Arka planda, sayı **3** başka bir dizeye gömülmeden önce bir dizeye dönüştürülür.

Kod **"Hello, #{name}!"**, yeni bir dize nesnesi oluşturur ve ardından mevcut dizeyi **"Ada"**buna gömer.

Öte yandan kod **"Hello, " + name + "!"**, üç yeni dize nesnesi oluşturur: önce dizeyi oluşturur **"!"**ve ardından onu mevcut dizeyle birleştirir **"Ada"**. Operatör , şimdi olan *yeni* bir dize **+** döndürür . Şimdi bu dize yeniden ile birleştirilir , bu da yine *yeni* bir dize oluşturur, .**"Ada!""Hello, ""Hello, Ada!”.**

***[ALT DİZELERİ BİRLEŞTİRİN](https://www.educative.io/courses/learn-ruby-from-scratch/JPKnDVvVGV9)***

```ruby
def string_producer(input_string)
result = "#{input_string}<3<3<3"
return result
end 
```

[DOLDURMA VE YASLAMA](https://www.educative.io/courses/learn-ruby-from-scratch/m288KzGxvpR) 

Bir dizeyi başka bir dize ile doldurarak yaslamanıza izin veren bir yöntem vardır .

```ruby
def justifying_and_padding(input_string)
width = input_string.lenght + 6 
result = input_string.ljust(width, "<3")
return result
end
```

[**DİZEYİ FLOAT’A DÖNÜŞTÜR**](https://www.educative.io/courses/learn-ruby-from-scratch/JPz1y4GNB3l)

```ruby
def string_to_num(input_string)
result = input_string.to_f
return result
end
```

Bunun Gibi Bir Sürü Yöntemden Bahsedebiliriz Bir Kaçı Şunlar:

to_i = Dizeyi Bir Tam Sayıya Dönüştürür.

to_f = String’i Bir Float’a Dönüştürür.

to_r = String’i Rasyonel Sayıya Çevirir.

to_c = String’i Karmaşık Sayıya Dönüştürür.

[BİR DİZE BAŞA EKLEYİN](https://www.educative.io/courses/learn-ruby-from-scratch/qVlBw6D69rR)

```ruby
def prepend_string(string1, string2)
result = string2.prepend(string1)
return result
end 
```

[**KARAKTERLERİ DİZEDEN KALDIRIN**](https://www.educative.io/courses/learn-ruby-from-scratch/xV92DVrB5Ez)

```ruby
def remove_chars(input_string, input_characters)
  result = input_string.delete(input_characters)
  return result
end
```

[**DOĞRU YANLIŞ 0 NESNELER**](https://www.educative.io/courses/learn-ruby-from-scratch/JYlmPjYqq3l)

“NİL” Hiçbirşeyi temsil etmez

True gerçeği

False ise yanlışı temsil eder.

[**SEMBOLLERLE ÇALIŞMAK**](https://www.educative.io/courses/learn-ruby-from-scratch/JYPn23Lzk6y)

Semboller Nelerdir??

*Semboller, kod olmaları dışında dizeler gibidir* . Semboller, dürüst olmak gerekirse, oldukça garip bir kavramdır ve onları tanıtıyoruz çünkü semboller o kadar sık ve yaygın olarak kullanılıyor ki, büyük olasılıkla başka bir yerde kodda kullanıldığını göreceksiniz.

Bir sembol şöyle yazılır: :something.

yani önünde iki nokta bulunan bir kelime var. Bu, normalde sembollerin boşluk içermediği anlamına gelir. Bunun yerine, birden fazla kelimeden oluşan sembollerimiz varsa, onları aşağıdaki gibi alt çizgilerle birleştiririz: :another_funny_symbol

Bir Symbol kelimenin önüne iki noıkta üst üste eklenerek bir nesne oluşturulur.

Semboller, veri değil kod olarak kabul edilen benzersiz tanımlayıcılardır.

Semboller, dizelerin özel sınırlı bir varyasyonudur.

Teknik Fark

Dizeler ile semboller arasındaki temel teknik farkı anlamak için şunu deneyelim:

```ruby
puts "a string".object_id.true           Çıktı: Yok
puts "a string".object_id.false
puts "a string".object_id.true
```

 Oluşturulan 3 dize tamamen aynı olsa da, oluşturulan her yeni dizenin farklı bir özelliği vardır object_id: Aynı metni içermelerine rağmen aslında farklı nesnelerdir.

```ruby
puts :a_symbol.object_id                 Çıktı: 987228                   
puts :a_symbol.object_id                        987228
puts :a_symbol.object_id                        987228                         
```

Ruby'nin, programınızı oluşturan evrende uçan **object_id**tüm nesneleri takip etmek için dahili olarak kullandığı benzersiz bir kimliktir. Örneğin Ruby, hangi nesnelerin hala yararlı olduğunu ve hangilerinin temizlenip atılabileceğini bilmelidir. Bu **object_id**, her bir nesneyi benzersiz bir kimlikle tanımlamanın bir yoludur.

[**DİZELERLE ÇALIŞMAK**](https://www.educative.io/courses/learn-ruby-from-scratch/B8PQG34BQ9Y)

Dizi diğer nesneleri depolayan bir nesnedir.

```ruby
[1, 2 , 3] Öğrneği bu üç sayıyı tutan basit bir dizedir.
```

```ruby
["Bir dize", 1, true, : symbol, 2] Dizeler her türlünesneyi içerebilir.
```

**Örneğin, dizileri bir dizide de saklayabilirsiniz: bu 2 boyutlu bir dizidir, tıpkı birçok satırı olan bir tablo gibi ve her satırın birçok hücresi (“nesneleri”) vardır.**

**Aşağıdaki örnekte, dış dizi tabloyu temsil eder ve her iç dizi bir satırı temsil eder. Her değer daha sonra bir hücreyi temsil eder. Aşağıdaki, bir telefondaki sayı tuşlarının yapısını temsil eden 2 boyutlu veya iç içe diziye bir örnektir:**

```ruby
[
  [1, 2, 3],         Dizilerin tanımlanmış bir sırası vardır.
  [4, 5, 6],         Ve her türlü nesneyi saklayabilir.
  [7, 8, 9],
  [0]
]
```

**Bir Dizeden Eleman Alma**

Diziler birçok farklı ve faydalı şekilde kullanılabilir, ancak en temel olanı belirli bir öğeyi konumuna atıfta bulunarak almaktır: 

*Lütfen bana öğeyi konumundan getirin 1!*

```ruby
words = ["one", "two", "three"]             Çıktı: two
puts words[1]
```

Bunun nedeni şudur: Bir dizideki ilk konum **0**, değil **1**. Yani konum **1**, birinci öğeye değil, ikinci öğeye atıfta bulunur.

• İlk satırdaki köşeli parantezler , verilen öğelerle (yani değişkene atanan ) bir nesne **oluşturmak** için kullanılır **.Arraywords**

• İkinci satırda, köşeli parantezler artık name değişkenine eklenir **words**. Bu , diziden bir eleman **aramak** istediğimiz anlamına gelir **words.**

```ruby
puts [1, 2, 3].first     Çıktı: 1
puts [1, 2, 3].last             3
```

**Eksik Öğeler**

Var olmayan bir öğeyi, örneğin dördüncü veya beşinci konumdaki (indeks) öğeyi almaya çalışırsak ne olur?

```ruby
words = ["one", "two", "three"]        Çıktı:
puts words[3]

puts words[4]
```

**nil** Doğru, "hiçbir şey" anlamına gelen geri dönüyoruz 

**Bir Dizeye Eleman Ekleme**

```ruby
words = ["one", "two", "three"]       Çıktı: One    
words << "four"                              Two                          
puts words                                   Three
                                             Four
```

Bu yazdırılır **four**: "Dört" dizesi diziye eklenmiştir. Ve şimdi konumunda oturduğundan, **3** ona kullanarak erişebiliriz **words[3]**

**Bir Öğeyi Konumuna Ayarlama**

Bir öğeyi belirli bir dizine de ayarlayabiliriz, örneğin:

```ruby
words = ["one", "two", "three"].        Çıktı:four
words[3] = "four"
puts words[3]
puts words
```

Aynı şekilde mevcut öğelerin üzerine de yazabilirsiniz. Örneğin bu, sözcüğü "uno"şu konuma ayarlar 0(yani üzerine yaz "one".

```ruby
words = ["one", "two", "three"].        Çıktı:Uno        
words[0] = "uno"
puts words[0]
puts words
```

Köşeli parantezlerin içinde boşluk olmadığına ve her virgülden sonra bir boşluk olduğuna dikkat etmeliyiz.

[DİZELERLE YAPABİLECEKLERİMİZ](https://www.educative.io/courses/learn-ruby-from-scratch/3j6mY8Mlr9A)

**Dizelerin Birleştirilmesi**

```ruby
result = ["one", "two"] + ["three", "four"] Çıktı: one two three four
puts result
```

**Dizelerin Farkı**

```ruby
result = [1,1,2,3,4]-[1,2].     Çıktı: 3
puts result.                           4
```

**Bir Dizenin Birden Çok Kopyasını Birleştirme**

```ruby
puts ["Ruby", "Monstas"] * 3.     Çıktı: Ruby 
                                         Monstas
                                         Ruby 
                                         Monstas
                                         Ruby 
                                         Monstas
```

**Dizelerin Kesişimi**

```ruby
puts ([1, 2, 3] & [2, 3, 4]) Çıktı: 2
																		3
```

**Dizelerle Denemek İçin Başka Harika Şeyler**

```ruby
puts("length is")
puts [1, 2, 3].length

puts("sort is")
puts [3, 1, 2].sort

puts("compact is")
puts [1, nil, 2, 3, nil].compact

puts("index is")
puts [4,9,20].index(9)

puts("rotate is")
puts [1, 2, 3, 4].rotate(2)

puts("transpose is")
puts [[1, 2, 3], [4, 5, 6], [7, 8, 9]].transpose

puts("join is")
puts ["We", "are", "one"].join(".")
```

```ruby
Çıktı:
length is
3
sort is
1
2
3
compact is
1
2
3
index is
1
rotate is
3
4
1
2
transpose is
1
4
7
2
5
8
3
6
9
join is
We.are.one
```

[BİR DİZE OLUŞTURUN](https://www.educative.io/courses/learn-ruby-from-scratch/3wNEpPPWYnr)

```ruby
input_string_1="Hello"
input_string_2="Howdy"
input_string_3="Hey"

result =["Hello","Howdy","Hey"]  Bu 3 dizeyi içeren bir dize oluşturun.
```

```ruby
def new_array (input_string1,input_string2,input_string3)
result = [input_string1, input_string2, input_string3]
return result
end
```

[ARAYA EKLEME](https://www.educative.io/courses/learn-ruby-from-scratch/7nMWXAmrKmO)

```ruby
input_string_1 = "ha"
input_String_2 = "he"

result = ["ha","he","ha","he","ha","he","ha","he","ha","he"]
```

```ruby
def interleaving(input_string_1,input_string_2) 
result=[input_string_1,input_string_2]*5
return result 
end
```

[**BİR İFADE YAPIN](https://www.educative.io/courses/learn-ruby-from-scratch/m77zZmPx6wE)** 

```ruby
Input_array = [1,2,3,4,5]
result = 1+2+3+4+5
```

```ruby
def make_expression (input_array)
result =[input_array].join("+")
return result
end
```

**[DİZEDEKİ BİR ÖĞEYİ DEĞİŞTİRİN](https://www.educative.io/courses/learn-ruby-from-scratch/m2yyVJBx4xE)**

```ruby
def replace_element(input_array).        Çıktı:99
  input_array[3] = 99
  return input_array[3]
end
```

**[BİR DİZENİN ÖĞELERİNİ ALMA VE YENİDEN BİRLEŞTİRME](https://www.educative.io/courses/learn-ruby-from-scratch/B88mjZr3Kz2)**

```ruby
array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
result = [2, 4, 6]
```

```ruby
def combine_elements(input_array)
  result=[input_array[1],input_array[3],input_array[5]]
  return result
end
```

[DİZEYİ TERSİNE ÇEVİRİN](https://www.educative.io/courses/learn-ruby-from-scratch/gx6OOGE5Z26)

```ruby
input_array = [1,2,3,4,5]
result = [5,4,3,2,1]
```

```ruby
def reverse_elements(input_array)
result = input_array.reverse
return result
end
```

[BİR ÖĞREYİ SİL](https://www.educative.io/courses/learn-ruby-from-scratch/gkXOz66M58l)

```ruby
input_array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
element = 6
input_array = [1, 2, 3, 4, 5, 7, 8, 9, 10]
```

```ruby
def delete_element(input_array,element)
input_array.delete(element)
  return input_array
end
```

**[HASHLERLE ÇALIŞMAK](https://www.educative.io/courses/learn-ruby-from-scratch/3jK3POjGqzx)**

**Bir Şeyi Diğeriyle Arayın:**

Karmalar, diğer nesneleri depolamak için kullanılabilecek çok kullanışlı ve yaygın olarak kullanılan başka bir şeydir.

Hashler hemen hemen şu şekilde çalışır.

Bir karma, anahtarlara değerler atar, böylece değerler anahtarlarına göre aranabilir.

Bir anahtara atanan bir değere de *anahtar/değer çifti* olarak atıfta bulunuruz . Bir karma, istediğiniz kadar anahtar/değer çiftine sahip olabilir.

**Bir Karma Oluşturma**

Ruby'de, bir değere bir anahtar atayarak onları ile **=>**ayırarak, bu anahtar/değer çiftlerini virgülle ayırarak ve her şeyi kaşlı ayraçlar içine alarak bir karma oluşturabilirsiniz..

```ruby
{ "one" => "eins", "two" => "zwei", "three" => "drei" }
```

Bu, 3 anahtar/değer çifti içeren bir karma tanımlar; bu, üç farklı anahtarı (dizeler, ve ) kullanarak üç değeri ( dizeler **"eins"**, ve ) arayabileceğimiz anlamına gelir .**"zwei""drei""one""two""three"**

Bu arada, Ruby topluluğu, bir anahtarı bir değerden ayıran sözdizimi biti için ***karma roket adını buldu, … bunu bilmenin oldukça havalı olduğunu düşünüyoruz :).*=>**

Anahtar/değer çiftleri listelenerek, karma roketlerle ayrılmış ve küme parantezleri içine alınarak bir karma oluşturulur.

Bir Değer Aranıyor

```ruby
dictionary = { "one" => "eins", "two" => "zwei", "three" => "drei" }
puts dictionary["one"]          Çıktı: eins
```

İlk satırda tanımlanan karmaya atıfta bulunmak için ikinci satırda bir değişken adını nasıl kullandığımızı biliyor musunuz?

Bu örnekte, **dictionary**ilk satırda tanımlanan bir karmadır. olan **["one"]** anahtarla ilişkili değeri arar . Bu değer ekrana gönderilecek olana iletilecektir .**" one""eins"puts.**

**Bir Tuşa Karşı Bir Değer Ayarlama**

Ayrıca, dizilerde olduğu gibi, mevcut bir Hash üzerinde anahtar/değer çiftleri ayarlamanın bir yolu vardır:

```ruby
dictionary = { "one" => "eins", "two" => "zwei", "three" => "drei" }
dictionary["zero"] = "null"
puts dictionary["zero"]              Çıktı: null
```

Aynı şekilde mevcut anahtar/değerlerin üzerine de yazabilirsiniz. Örneğin, bu, sözcüğü **"uno"**anahtara ayarlar **"one"**(yani, değeri olan mevcut çiftin üzerine yazar **"eins"**):

```ruby
dictionary = { "one" => "eins", "two" => "zwei", "three" => "drei" }
dictionary["one"] = "einss"
puts dictionary["one"]               Çıktı: einss 
```

**Her Türlü Nesne**

Her türlü nesneyi anahtar olarak kullanabilir ve her türlü nesneyi değer olarak saklayabilirsiniz. Örneğin, bunların hepsi de geçerli karmalardır:

```ruby
{ 1 => "eins", 2 => "zwei", 3 => "drei" }
{ :one => "eins", :two => "zwei", :three => "drei" }
{ "weights" => ["pound", "kilogram"], "lengths" => ["meter", "mile"] }
{ :de => { :one => "eins", :two => "zwei", :three => "drei" } }
```

İlk örnek, sayıları anahtar olarak kullanırken, ikincisi Ruby'de oldukça yaygın olan sembolleri kullanır.

Üçüncü örnekte, dizilerin karmalarda değerler olarak kullanılabileceğini görebilirsiniz. Yani anahtarı ararsanız, **"weights"**şimdi bir dizi geri alırsınız.

*Son satır aslında Rails'in* dizeleri farklı dillere çevirmek için kullandığı şeye oldukça yakındır : Aynı zamanda bir "iç içe karma" örneğidir. **:de** Anahtar için (Almanca dilini temsil eden ) bir değer olarak ilişkilendirilmiş (depolanmış) başka bir karma vardır . Ve bu diğer karma artık üç anahtar/değer çiftine sahip. Böylece bir *Rails* programcısı "one" kelimesini Almancaya nasıl çevireceğini araştırabilir ve "eins"i geri alabilir.

**Hash'ler, her türlü nesneyi anahtar ve değer olarak kullanabilir.**

**Eksik Değerler**

Var olmayan bir anahtarı aramaya çalışrısak ne olur?

nil. Yine dizelerde olduğu gibi, “hiçbirşey” anlamına gelen’i geri döneceğiz.

```ruby
dictionary = { "one" => "eins", "two" => "zwei", "three" => "drei" }
puts dictionary["four"]                   Çıktı: 
```

**[HASH İLE YAPABİLECEKLERİMİZ](https://www.educative.io/courses/learn-ruby-from-scratch/JYQJDm0NJxl)**

**Hashlerde Günlük Yöntemler**

**Birleştirme**

merge Yöntemini çağırarak iki karmayı birleştirebilirsiniz.

```ruby
dictionary={ "one" => "eins" }.merge({ "two" => "zwei" })
puts dictionary              Çıktı: {"one"=>"eins", "two"=>"zwei"}
```

Fetch

fetchdaha önce tartışılan köşeli parantez aramasıyla aynı şeyi yapar [ ], ancak anahtar tanımlanmadıysa bir hataya neden olur:

```ruby
dictionary = { "one" => "eins" }                 Çıktı: eins 
puts dictionary.fetch("one")                            hata verir.
puts dictionary.fetch("two")
```

**Keys**

**keys** Bir karmanın bildiği tüm anahtarları içeren bir Dize döndürür:

```ruby
dictionary = { "one" => "eins", "two" => "zwei" }
puts dictionary.keys                 Çıktı: One
                                            Two
```

**Length and Sıze**

**length** ve **size** ikisi de karmada kaç anahtar/değer çiftinin bulunduğunu söyler:

```ruby
dictionary = { "one" => "eins", "two" => "zwei" }
puts dictionary.length           Çıktı: 2
puts dictionary.size                    2
```

**[HASH SÖZDİZİMİ KARIŞIKLIĞI](https://www.educative.io/courses/learn-ruby-from-scratch/3jEpExDzpo9)** 

**Eski Söz Dizimi**

```ruby
{ one: "eins", two: "zwei", three: "drei" }
```

**Yeni Söz Dizimi**

```ruby
puts hash = { :one => "eins", :two => "zwei", :three => "drei" }
puts hash1 = { one: "eins", two: "zwei", three: "drei" }
```

**Keys’leri Elde Etme** 

```ruby
def return_hash(dictionary,key)
    dictionary = {:one => 'one', :two => 'two', :three => 'three'}
    result=dictionary.keys
    return result
end
```

**Keys’lerle Değerler’in Yerini Değiştirme** 

```ruby
def flip_keys_vals(input_hash)
  result = input_hash.invert
  return result
end
```

[**NESNELER SINIFLAR VE YÖNTEMLER**](https://www.educative.io/courses/learn-ruby-from-scratch/NEYlrBoxrmK)

Ruby’de Herşey Bir Nesnedir.

Ruby’de hemen hemen herşey bir nesnedir.

**[NESNELER SINIFLARIN ÖRNEKLERİDİR](https://www.educative.io/courses/learn-ruby-from-scratch/qVANmDRj84r)**

Nesnelerin Sınıfları Vardır.

Daha [önce](https://www.educative.io/collection/page/10370001/5658174447157248/5681589568667648) de belirtildiği gibi , bir Ruby programını çalıştırdığınızda, programınız tarafından tanımlanan somut nesnelerle (şeyler) küçük bir evren (uzay) oluşturulur ve doldurulur. Bu şeyler, çağırdığınız belirli yöntemleri kullanarak etkileşime girer ve faydalı şeyler yapar.

**Böyle bir nesneyi sınıfı için sorduğunuzda nesnelerin sınıfları olduğunu görebilirsiniz:**

```ruby
print "this is a string".class.        Çıktı: string
```

**Aynı soruyu Ruby'de sormanın başka bir yolu:**

```ruby
print "this is a string".is_a?(Numeric).   Çıktı: False
```

[**YÖNTEMLER**](https://www.educative.io/courses/learn-ruby-from-scratch/m22E72p1mL9)

*Yöntemler bir nesnenin davranışıdır*

Nesnelerin, onlarla ilginç şeyler yapmamızı sağlayan yöntemleri vardır. Bir nesnenin yöntemleri, nesnenin yapabileceği *şeylerdir.*

Birini düşün, bir arkadaşın gibi. Bu kişiye adını sorabilirsiniz (bir yöntem çağırın) ve size söyleyecektir (size geri verin). İsimleri, bu kişinin sahip olduğu bir bilgi parçasıdır ve bunu size söyleme (sorunuza cevap verme) yeteneği, sahip oldukları bir davranış (yöntem) parçasıdır.

[**ÇAĞRI YÖNTEMLERİ**](https://www.educative.io/courses/learn-ruby-from-scratch/JYWBVNwxyGg)

Ruby'de, nesneler üzerinde tanımlanan yöntemler bir nokta ve ardından yöntem adı eklenerek kullanılabilir, örneğin:

```ruby
object.method
```

```ruby
name = "Ruby Monstas"
                                   Çıktı:
puts name.upcase.                         RUBY MONSTAS
puts name.downcase.                       ruby monstas
puts name.lenght.                         12
```

Ve bunun gibi.
Başka bir deyişle, önce konuşmak istediğiniz nesneyi adreslersiniz veya bahsedersiniz ve ardından nokta ile **.** yöntem adını belirterek nesneye “mesaj gönderirsiniz”. Biz de diyoruz ki: “yöntemi string üzerinde büyük harf olarak çağırırsınız”.

Bir nesne üzerinde bir yöntemi çağırmak için bir nokta kullanılır.

Diğerleri nesnenin kendisini değiştirir ve bazılarının yan etkileri vardır ve başka bir şeyi değiştirir, örneğin **puts**ve **p** her ikisi de ekrana bir şeyler verir. Diğer yöntemler dosyaları kaydedebilir, e-posta gönderebilir veya bir veritabanında bir şeyler depolayabilir.


[ARGÜMANLARI GEÇMEK](https://www.educative.io/courses/learn-ruby-from-scratch/m2qGXRR9G6A)

## **Ekstra bilgi gerekli [#](https://www.educative.io/courses/learn-ruby-from-scratch/m2qGXRR9G6A#Extra-information-needed)**

Bazen bir nesne, istediğinizi yapmak için biraz fazladan bilgiye ihtiyaç duyar.

Örneğin, sınıf , bazı karakterleri silinmiş olarak başka bir String döndüren **String** yöntemi tanımlar . **delete** Bunu yapabilmek için elbette hangi karakterleri kaldırmak istediğimizi bilmesi gerekiyor.

**()** Metot çağrısına (isim) parantez koyarak bazı şeyleri iletebiliriz . Daha sonra gerekli olan fazladan bilgiyi (bizim durumumuzda başka bir dize) parantez içine şu şekilde ekleyebiliriz:

```ruby
puts name = "Ruby Monstas"    Çıktı: Runstas
puts name.delete("by Mo")
```

Argüman gerektiren bir yönteme başka bir örnek, **prepend** Strings'deki yöntemdir:

```ruby
puts name = "Ruby Monstas"       Çıktı: Ruby Monstas
puts name.prepend("Oh Hello ")          Oh Hello Ruby Monstas 
```

Tüm yöntemlerin işlerini yapmak için bu ekstra bilgi bitlerine (argümanlara) ihtiyacı yoktur, örneğin, **length.**Strings'deki yöntem.


[LİSTELEME YÖNTEMLERİ](https://www.educative.io/courses/learn-ruby-from-scratch/NE7kO82X5Gz)

Nesneden yöntemlerini hızlı bir şekilde isteyebilirsiniz. Bu doğru, **methods** tüm nesnelerde tanımlanmış bir yöntemdir (tıpkı **class**ve gibi **is_a?**).

Onu çağırdığınızda, nesnenin sahip olduğu tüm yöntem adlarını içeren bir dizi döndürür (yanıt verir).

Diziyi sıralamak mantıklıdır, bu nedenle okunması daha kolaydır. Şöyle:

```ruby
print "Ruby Monstas".methods.sort 
Çıktı: [:!, :!=, :!~, :%, :*, :+, :+@, :-@, :<, :<<, :<=, :<=>, :==, :===, :=~, :>, :>=, :[], :[]=, :__id__, :__send__, :ascii_only?, :b, :between?, :bytes, :bytesize, :byteslice, :capitalize, :capitalize!, :casecmp, :center, :chars, :chomp, :chomp!, :chop, :chop!, :chr, :class, :clear, :clone, :codepoints, :concat, :count, :crypt, :define_singleton_method, :delete, :delete!, :display, :downcase, :downcase!, :dump, :dup, :each_byte, :each_char, :each_codepoint, :each_line, :empty?, :encode, :encode!, :encoding, :end_with?, :enum_for, :eql?, :equal?, :extend, :force_encoding, :freeze, :frozen?, :getbyte, :gsub, :gsub!, :hash, :hex, :include?, :index, :insert, :inspect, :instance_eval, :instance_exec, :instance_of?, :instance_variable_defined?, :instance_variable_get, :instance_variable_set, :instance_variables, :intern, :is_a?, :itself, :kind_of?, :length, :lines, :ljust, :lstrip, :lstrip!, :match, :method, :methods, :next, :next!, :nil?, :object_id, :oct, :ord, :partition, :prepend, :private_methods, :protected_methods, :public_method, :public_methods, :public_send, :remove_instance_variable, :replace, :respond_to?, :reverse, :reverse!, :rindex, :rjust, :rpartition, :rstrip, :rstrip!, :scan, :scrub, :scrub!, :send, :setbyte, :singleton_class, :singleton_method, :singleton_methods, :size, :slice, :slice!, :split, :squeeze, :squeeze!, :start_with?, :strip, :strip!, :sub, :sub!, :succ, :succ!, :sum, :swapcase, :swapcase!, :taint, :tainted?, :tap, :to_c, :to_enum, :to_f, :to_i, :to_r, :to_s, :to_str, :to_sym, :tr, :tr!, :tr_s, :tr_s!, :trust, :unicode_normalize, :unicode_normalize!, :unicode_normalized?, :unpack, :untaint, :untrust, :untrusted?, :upcase, :upcase!, :upto, :valid_encoding?]
```

Evet, yöntem adları Sembol olarak gelir, çünkü bunlar kod olarak kabul edilir.

**Zincirleme Yöntem Çağrıları**

String örneğimizden bazı yöntem çağrılarını şu şekilde zincirleyebiliriz:

```ruby
name = "Ruby Monstas"              Çıktı: OH, HELLO, RUBY MONSTAS
puts name.prepend("Oh, hello, ").upcase
```

Oldukça kullanışlı.

Gördüğünüz gibi Ruby önce biti değerlendirecek,         

**name.prepend("Oh, hello, ")**. Bundan döndürülecek nesneyi (yeni Dize) bilmesi için bunu yapması gerekir, böylece daha sonra **upcase** bu yeni nesne üzerindeki yöntemi çağırabilir.


[YÜKLEMLER](https://www.educative.io/courses/learn-ruby-from-scratch/B86JvDn0GZn)

**Tahmin Yöntemleri**

Kural olarak, Ruby'de bu yöntemler ya **true** veya **false**. Örneğin, bir sayının çift mi yoksa tek mi olduğunu sorabiliriz;

```ruby
puts 5.odd?                    Çıktı: True 
puts 5.even?                          False
```

Veya numaranın diğer iki numara arasında olup olmadığını sorabilirsiniz. Açıkçası bu yöntemin diğer iki sayıyı geçmemize ihtiyacı var. Şimdi elimizde iki argüman alan bir yöntem örneğimiz de var:

```ruby
puts 5.between?(1, 10)          Çıktı: True
puts 5.between?(11, 20)                False
```

Bu yöntemlere Ruby'de **Yüklem Yöntemleri** denir.

İçine Dahil Mi?

```ruby
name = "Ruby Monstas"          Çıktı: True 
puts name.include?("by")              False
puts name.include?("r")
```

Dizilerin yöntemleri vardır **include?** ve Hash'ler şunlara yanıt verir **key?**:

```ruby
puts [1, 2].include?(1)          Çıktı: True

puts [1, 2].include?(3)                 False

puts ({ "eins"=>"one" }.key?("eins"))   True

puts ({ "eins" => "one" }.key?("zwei")) False
```

Bir sayı üzerinde hangi yöntemlerin tanımlandığını kontrol ettiğimizde, bazı ilginç olanları buluruz:

```ruby
print 1.methods.sort
Çıktı: [:!, :!=, :!~, :%, :&, :*, :**, :+, :+@, :-, :-@, :/, :<, :<<, : <=, :<=>, :==, :===, :=~, :>, :>=, :>>, :[], :^, :__id__, :__send__, :abs, :abs2 , :açı, :arg, :arasında?, :bit_length, :ceil, :chr, :class, :clone, :zorlama, :conj, :conjugate, :define_singleton_method, :payda, :display, :div, :divmod, :aşağı, :dup, :enum_for, :eql?, :equal?, :even?, :extend, :fdiv, :floor, :freeze, :frozen?, :gcd, :gcdlcm, :hash, :i, : imag, :imaginary, :instance_exec, :instance_eval, :instance_exec, :instance_of?, :instance_variable_defined?, :instance_variable_get, :instance_variable_set, :instance_variables, :tamsayı?, :is_a,::, :itself büyüklük, :yöntem, :yöntemler, :modulo, :negatif?, :sonraki, :nil?, :sıfır olmayan?, :pay, :object_id, :tek?, :ord, :faz, :polar, :pozitif?, : pred, :özel_yöntemler, :korumalı_methods, :public_method, :public_methods, :public_send, :quo, :rasyonalize, :gerçek, :gerçek?, :doğru, :dikdörtgen, :kalan, :remove_instance_variable, :respond_to?, :yuvarlak, :send_, :send, singleton_method, :singleton_method_added, :singleton_methods, :size, :step, :succ, :taint, :tainted?, :tap, :times, :to_c, :to_enum, :to_f, :to_i, :to_int, :to_int, : , :kesin, :güven, :untaint, :güvenilmez, :güvenilmeyen?, :upto, :sıfır?, :|, :~]güvenilmeyen?, :upto, :sıfır?, :|, :~]güvenilmeyen?, :upto, :sıfır?, :|, :~]
```

[PATLAMA](https://www.educative.io/courses/learn-ruby-from-scratch/3jO392nvxDQ)

**Patlama Yöntemleri** 

Bunlar sorulardır ve çağrıldıkları nesneyi değiştirmezler.

```ruby
name = "Ruby Monstas"          Çıktı: ruby monstas
puts name.downcase                    Ruby Monstas
puts name
```

Yukarıdaki kod satırlarını çalıştırırsanız, yöntemin **downcase** orijinal Dize'nin küçük harfli versiyonu olan yeni bir Dize döndürdüğünü göreceksiniz. Orijinal String'i bir sonraki satırda çıkardığımızda, bunun hala aynı olduğunu görebiliriz: Yöntem **downcase** String'i değiştirmez.

**! İle Biten Yöntemler**

Ancak, bu yöntemlerden bazılarının ünlem işaretiyle biten çeşitleri de vardır **!**. Bu yöntemlere **"bang yöntemleri"** denir ve genellikle çağrıldıkları nesneyi değiştirirler.

Örneğin, yönteme ek olarak, **downcase** Dizelerin bir yöntemi de vardır **downcase!**

```ruby
name = "Ruby Monstas"         Çıktı: ruby monstas
puts name.downcase!                  ruby monstas
puts name
```

Gördüğünüz gibi **downcase!**, ikinci satırdaki yöntemi çağırmak, String'in kendisini (başvurulan nesne **name**) değiştirdi ve *ayrıca* yeni küçültülmüş sürümü döndürdü.


[YÖNTEMLER](https://www.educative.io/courses/learn-ruby-from-scratch/m22EWQlJEkn)

## **Yöntemlerin önemi**

Programlamadaki her şey verilerle ve onunla ilginç şeyler yapmakla ilgilidir. Twitter'ı düşünürseniz, esasen kullanıcılarından 140 karakterlik metin (veri) alır ve başkalarına gösterir.

Ruby'deki en önemli ilkel (basit) veri türlerini zaten öğrendiniz: sayılar, dizeler, true, false ve nil. Ve en yaygın iki veri yapısına, Dizilere ve Karmalara bir göz attık.

Bütün bunlar *veri* kısmıyla ilgili. Yöntemler ise *ilginç şeyler yapmakla* ilgilidir .

Bu bölümde, bir yöntemin anatomisine daha yakından bakacağız ve kendi yöntemlerinizi nasıl uygulayacağınızı ve kullanacağınızı öğreneceğiz.

bu bölümden sonra sizde kendi yönteminizi ıufılayavşikceksiniz

## **Yöntemler davranışı tanımlar**

Yöntemlerin tamamı *davranışı* tanımlamakla ilgilidir , böylece farklı bağlamlarda farklı veri bitlerine kolayca uygulanabilirler.

Örneğin, bir dizeyi dönüştürmek, bir diziyi sıralamak, bir **CSV** veya bir **Excel** dosya okumak, bir e-posta göndermek, Facebook'ta oturum açmak, bir Tweet göndermek gibi şeyler yapan yöntemler vardır.

Bunu koymanın başka bir yolu da şudur: Yöntemler, belirli bir kod parçasına bir ad atamanın bir yoludur. Tıpkı bir değişkenin bir nesneye "aramamızı" veya bir nesneye başvurmamızı sağlaması gibi, yöntemler o nesneyle ilişkili kod parçalarını yürütmemizi sağlar.

Değişkenler nesneleri, yöntemler ise davranışı (kod) adlandırır.

Yöntemler, kodu paketleme ("kapsülleme") ve üzerine bir isim yapıştırma yoluyla kodu yeniden kullanılabilir hale getirir.

Gördüğünüz gibi Ruby, deneyimli programcılar tarafından yazılmış, önceden tanımlanmış birçok yöntemle birlikte gelir. Bu nedenle, bilgisayar bilimi eğitimi almıyorsanız ve veri toplama için kendi karmaşık sıralama algoritmalarınızı uygulama alıştırmasıyla karşı karşıya değilseniz **sort**, Ruby'de Diziler için kutudan çıktığı haliyle zaten tanımlanmış olan yöntemi kullanacaksınız.


[BİLEŞENLER](https://www.educative.io/courses/learn-ruby-from-scratch/7AVRYBjQKnQ)

 

### **Argümanlar ve dönüş değerleri**

Programcılar genellikle bu bağlamda "girdi" terimini kullanmazlar. Bunun yerine, bir yöntemin bir dizi argümanı (girdi parçaları) kabul ettiğini söylüyoruz. Ve “çıktı” yerine dönüş değeri terimini kullanıyoruz: yöntemden geri aldığımız şey.

### A**naloji**

Biraz para koyabileceğiniz, bazı düğmelere basabileceğiniz ve makinenin birkaç dişli ve çarkı döndüreceği ve peşinde olduğunuz çikolatayı tüküreceği bir otomat hayal edin.

Otomat bir yöntem olsaydı, o zaman paranız ve bastığınız düğmeler ***girdidir*** . Makinenin belirli mekaniği dahili olarak döndürme şekli, ***kod bloğudur*** , dahili olarak yaptığı şeydir. Ve dağıttığı ürün ***iade değeridir*** .

Programcı olmayan biri için bundan bahsetmek garip gelse de, bir otomat makinesinin parayı ve verileri çikolataya “dönüştürmenin” bir yolu olduğunu söyleyebiliriz.

Yöntemlerin bir adı vardır, bazı girdiler alır, onunla bir şeyler yapar ve bir sonuç döndürür.

Bir yöntemin girdisine “argümanlar”, çıktısına ise “dönüş değeri” denir.

[YÖNTEM TANIMI](https://www.educative.io/courses/learn-ruby-from-scratch/7nWAA8l1JVj)

## **Tek başına yöntemler [#](https://www.educative.io/courses/learn-ruby-from-scratch/7nWAA8l1JVj#Stand-alone-methods)**

Şimdiye kadar nesneler üzerinde tanımlanan ve nesneler üzerinde çağrılabilen yöntemler gördünüz. **downcase** örneğin, her dizede tanımlanan yöntemi gördünüz .

Ancak Ruby, bu nesnelerin hiçbirinde tanımlı olmayan yöntemlere de izin verir. Bir nevi *bağımsız* yöntemlerdir.

Örneğin, şunu deneyebilirsiniz:

```ruby
puts is_a?(1)
```

**Yöntem Tanımlama**

Bir sayı alan, ona sayıyı ekleyen ve sonucu döndüren basit bir yöntem tanımlamamız gerektiğini varsayalım.Bunu şu şekilde yapabiliriz:

```ruby
def add_two(number)
number + 2
end
```

Bu bir yöntemi *tanımlar .* Henüz *kullanmıyor* : O otomat makinesini yalnızca yapar ve yerleştirirsiniz, böylece daha sonra (kendiniz veya başkaları tarafından) kullanılabilir.

Bu yöntem tanımını adım adım inceleyelim:

- Ruby üstteki kodu okumaya başlayacak ve anahtar kelimeyi bulacaktır **def**. Bu Ruby'ye yeni bir yöntem tanımlamak üzere olduğumuzu söyler.
- Yöntemlerin bir ada ihtiyacı vardır, bu nedenle Ruby sonra onu arar ve kelimeyi bulur **add_two**.
- **Ruby daha sonra yönteme “girdi”** olarak hizmet edecek herhangi bir şey tanımlayıp tanımlamadığımızı kontrol eder (unutmayın, bu isteğe bağlıdır). Parantezleri buluyor ve yönteme verilebilecek şeylerin bir listesini tanımlamak üzere olduğumuzu biliyor. *Bu listeye argüman listesi* denir .

 Bir bağımsız değişken listesi, yönteme iletilen nesnelerin adlarını, yöntem adından hemen sonra parantez içine alınmış olarak tanımlar.

- Bizim durumumuzda, argüman listesi tek bir argümana sahiptir **number**, bu da yöntemimizin tek bir şeyi (nesneyi) kabul edebileceği anlamına gelir.
- Sonraki satır, yöntemimizin sahip olduğu kod bloğudur (veya "kapsüllediği kod"). Bu aynı zamanda *yöntem gövdesi* olarak da adlandırılır . Bizim durumumuzda, bu sadece tek bir satır çünkü yöntemimizin kapsadığı işlem çok basit. Diğer yöntemler (düşün **sort**, Dizilerde tanımlanmış) daha fazla kod gerektirir ve daha uzundur.
- Yöntem gövdesinin içinde argümanlar *yerel değişkenler* olarak bilinir : Yöntem gövdemizdeki kodun değişken adını nasıl kullandığını görebilirsiniz **number**.
- Son olarak anahtar sözcük **end** Ruby'ye yöntem gövdesi ve yöntem tanımıyla işimizin bittiğini söyler.

Şimdiye kadar yaptığımız tek şey yöntemi tanımlamak, henüz hiçbir şey için kullanmadık. Bunu bir sonraki bölümde yapacağız.

[KULLANIM](https://www.educative.io/courses/learn-ruby-from-scratch/gxklVMz378l)

**Bir Yöntemi Çağırmak**

Bir metot tanımlandıktan sonra onu kullanabiliriz. Programcılar olarak genellikle bir metot *çağırdığımızı* söyleriz . Bu, Ruby'den yöntem gövdesinin sahip olduğu kodu, verilen bazı argümanlarla (varsa) yürütmesini istediğimiz anlamına gelir.

İşte nasıl göründüğü:

```ruby
def add_three(number).             Çıktı: 5
  number + 2
end

puts add_three(3)
```

AÇIKLAMA (KOD BRİFİNGİ)

Burada neler olduğunu mikroskop altında inceleyelim. Henüz bunun her bir parçasını anlamadıysanız, endişelenmeyin, bunların tümüne geri döneceğiz.

İlk üç satırda Ruby, yöntemi **add_two** daha önce tartışıldığı gibi tanımlar. Satır **4** kod içermez, bu nedenle Ruby onu görmezden gelir.

- On line **5** Ruby önce parçaya bakacaktır **add_two(3)**. Daha önce tanımlanmış bir yönteme atıfta bulunduğumuzu anlıyor ve bu ona bu yöntemi çağırmak (yürütmek) istediğimizi söyleyecek.
- Bunu yapmak için, önce parantez içinde ne olduğuna bakması gerekiyor, **()** böylece aktarabiliyor. 'ı bulur **3**. Bu noktada yeni bir yerel değişken yaratır **number** ve ona 3 sayısını atar.
- Şimdi Ruby, sayıyı geçen yöntem gövdesini yürütmeye başlamaya hazır **3**.
- Yani Ruby şimdi dosyamızda yukarıdan aşağıya doğru giden normal akıştan sapıyor. Bunun yerine, şimdi yöntem gövdesine atlıyor.

Yöntem *bağımsız değişkenleri* şu şekilde çalışır:

Bir yöntem çağrıldığında ve nesneler argüman olarak iletildiğinde, Ruby dolaylı olarak yerel değişkenleri argüman isimleriyle tanımlar. Geçirilen nesneleri argüman listesindeki değişken isimlerine atar. Bu yerel değişkenler daha sonra yöntem gövdesinde bulunur.

Bizim durumumuzda, sadece bir argümanımız var **number**. **number** Böylece nesnenin atandığı bir yerel değişken elde ederiz **3** (çünkü yöntemi çağırdığımızda iletilen nesne budur).

Yöntem gövdesinin şimdi şöyle okuduğunu hayal edebiliriz:

```ruby
number = 3
return number + 2
```

Tamam, şimdi yöntem gövdesinin içindeyiz:

- Ruby şimdi yöntem gövdesini yürütecek (değerlendirecek, çalıştıracak) (yine yukarıdan aşağıya doğru gidiyor), ki bu bizim durumumuzda return ifadesiyle yalnızca tek bir satırdır **number + 2**
- • Atandığı **number** için **3** ifade **number+2** olarak değerlendirilir **5** ve bu, yöntem çağrısından döndürülecek değerdir.

Yani Ruby şimdi yöntemin dışına çıkıyor. İfade **add_two(3)** az önce nesneyi döndürdü **5**. Bunun yerine son satırın şimdi şöyle olduğunu hayal edin:
```ruby
puts 5
```

**DÖNÜŞ DEĞERLERİ**

Ruby'de bir yöntem her zaman tam olarak tek bir şey (bir nesne) döndürür.

Döndürülen nesne herhangi bir şey olabilir.

Döndürülen nesne **nil**, "hiçbir şey" anlamına gelen nesne olabilir. Öte yandan, bir sürü şeyi aynı anda döndürmek için ilgilendiğimiz şeyleri tutan bir Dizi döndürebiliriz, ancak Dizinin kendisi yalnızca bir nesnedir.

**Her yöntem her zaman tam olarak bir nesne döndürür.**

## **İade beyanı yok!**

**return** Ayrıca Ruby'de diğer dillerde olduğu gibi deyimini kullanmak zorunda olmadığımızı da unutmayın . Aslında, çoğu Ruby kodu anahtar kelimeyi hiç kullanmaz **return**.

Bu son derece kullanışlıdır, ancak aynı zamanda öğrenmemiz gereken bir şeydir:

Bir yöntemin içine bir dönüş ifadesi koymazsak, yine de bir nesne döndürür: yöntem her çalıştırıldığında, yöntem gövdesinin son değerlendirilen ifadesinden üretilen nesneyi döndürür.

Bunu anlamak önemlidir. Bu yüzden tekrar ifade ediyoruz:

Açıkça hiçbir şey döndürmezsek, bir yöntem yine de son değerlendirilen ifadenin dönüş değerini döndürür.

Bir önceki örneğimizde…

```ruby
def add_two(number).         Çıktı: 5
number + 2
end 

p add_two(3)
```

… son değerlendirilen ifade ifadedir **number + 2**. Örneğimizde bu ifade **number** atandığı **3** için sayıyı döndürür **5** ve bu nedenle yöntemimiz tarafından döndürülen değer de **5**.

Bazen yöntemden erken “dönmek” isteriz. Aslında, bunu **return** ifadeyi kullanarak yapabiliriz. Ancak şimdilik, bu dava için endişelenmenize gerek yok.

[KAPSAMLAR](https://www.educative.io/courses/learn-ruby-from-scratch/gx89WpnBllD)

[**YÖNTEMLERİ BİRLEŞTİRME**](https://www.educative.io/courses/learn-ruby-from-scratch/gxpBBnOWEJl)

Diğer metodlardan metodları çağırabiliriz.

Başka Bir Yöntemden Arama Yöntemleri

Örneğin, yöntemimizi add_two başka bir yöntem kullanarak yeniden yazabilir add_one ve onu iki kez çağırabiliriz.

```ruby
def add_one(number).                    Çıktı: 5
number + 1
end
def add_two(number)
number = add_one(number)
add_one(number)
end 

puts add_two(3)
```

Ruby’de tüm bu şeyi sadece “+” operatörü kullanarak da çözebiliriz.

“+” Ancak , örnek için, operatörle tamamen aynı şeyi yapan bir yöntemi nasıl ekleyebileceğimize bir göz atalım:

```ruby
def sum(number, other).      puts sum(3, 8.5)      Çıktı: 11.5
number + other
end
```

Bu örnekte yöntemimizin sum şimdi iki argüman aldığını ve bu nedenle onu çağırdığımızda iki sayı iletmemiz gerektiğini unutmayın.

```ruby
def sum(number, other).                           Çıktı: 4
  number + other                                         5
end

def add_one(number)
  sum(number, 1)
end

def add_two(number)
  sum(number, 2)
end

puts add_one(3)
puts add_two(3)
```


[**BASKI İŞLEMLERİ**](https://www.educative.io/courses/learn-ruby-from-scratch/RL8XjQg5EzY)

Terminale birşeyler veren kısa bir Ruby programı çalıştırmayı içerir.Şimdiye kadar, çoğunlukla puts bunu yapmak için yöntemi kullandık.

Bu yöntem yöntemdir **p**. Daha iyi anlamak **p** için önce başka bir metoda bakmak istiyoruz ki bu metod **inspect**.

Inspect yöntemi, Ruby’deki herhangi bir nesnede kullanılabilir.Nesnenin kendisinin temsili olan bir dize döndürür: nesneyi oluşturmak için kullandığınız koda mümkün olduğunca yakın bir temsil.

```ruby
puts 5.inspect.                     Çıktı: 5

puts "A string".inspect

puts [1, 2, 3].inspect
```

Gördüğünüz gibi, döndürülen dize **inspect**, nesneyi oluşturmak için kullandığımız Ruby koduyla tamamen aynıdır.

Ancak, yazmak **puts something.inspect** oldukça zor bir iştir.Bu, nesnenin yanına yazılacak 12 karakterdir.

Bu yöntem şöyle uygulanır:

```ruby
def p(object)
puts object.method
end
```

Belirli bir kod satırının ne yaptığını, bir değişkene ne atandığını veya bir yöntem çağrısının ne döndürdüğünü anlamaya p çalıştığınızda, size tam olarak aradığınız şeyin ne olduğunu söylediği için kullanımını öneririz.

puts diğer yandan akıllı olmaya çalışır.

Örneğin, bir dizeye ilettiğinizde, puts o zaman nesnelerin her birinin çıktısını ayrı bir satırda verir:

```ruby
something = [1, 2, 3].                
puts something                         
p something 
```

```ruby
Çıktı: 1
2
3
Çıktı: [1, 2, 3]

```

Ayrıca, sayıları ve sayıları içeren dizelerin çıktısı, kullandığınızda tamamen aynıdır puts:

```ruby
puts 123                   Çıktı: 123 
puts "123"                        123
                                  
p "123"                           "123"

```

Çıktısından, **puts** aradığınız nesnenin sayılar içeren bir dizi mi yoksa dizeler içeren bir dizi mi yoksa yalnızca satır sonları içeren uzun bir dize mi olduğu genellikle net değildir.

Kısacası, **puts** ekrana gerçekten bir şey çıkarması gereken bir program yazarken kullanışlıdır.

Bu, işinizde kendi hayatınızı kolaylaştırmak için yazdığınız bir komut satırı aracı olabilir ve bu,

bazı tekrarlayan işleri otomatikleştirmeye yardımcı olur. Ya da Ruby programlama alıştırmalarında işe yarar. Öte yandan, p kodunuzun nen yaptığını anlamaya çalışırken, örneğin belirli bir hatayı bulmaya çalışırken yararlıdır.

# Yürütme Akışı

**[YÜRÜTME AKIŞI](https://www.educative.io/courses/learn-ruby-from-scratch/RMjPL4NGDlO)** 

Bir Ruby dosyasını çalıştırdığınızda (ruby runtime ile) Ruby kodunuzu okuyacak ve yukarıdan aşağıya satır satır yürütmeye başlayacaktır.

Örnek

Örneğimize yukarıdan ve Ruby kontrol akışının mikroskop altında nasıl geçtiğine bakalım.

puts Pratikte buna karışı önermemize rağmen, bunu daha açık hale getirmek için yöntem çağrısına

parantez ekledik:

```ruby
def add_two(number).                  Çıktı: 5
number + 2
end 
puts (add_two(3))
```

KOD BRİFİNGİ

Ruby 1.satırdan başlar ve anahtar kelime ile başlayan yöntem tanımımızı bulur **def**, bu nedenle 3. satırdaki anahtar kelimeyi bulana kadar hepsini okuyacaktır end.Şimdilik, bu yöntemi tanımlamaktan ve bellekte tutmaktan başka birşey yapmıyor. Şu andan itibaren kullanılabilir.

Şimdi 5.satırda, Ruby kelimeyi kullandığımızı buluyor puts ve ona bir şey iletmeye çalıştığımızı görüyor, bu yüzden bu bir yöntem çağrısı olmalı.

Bir metodu çağırmak için Ruby önce iletmek istediğimiz değerleri değerlendirmesi gerekir.Böylece Ruby şimdi parantezler arasında ne olduğuna bakar ve başka bir çağrı yöntemi bulur add_two(3).

Yine, yöntemi gerçekten çağırmak için add_two Ruby’nin önce iletmek istediğimiz değerleri değerlendirmesi gerekiyor.

Bu durumda, bu sayıdır 3, dolayısıyla Ruby bu nesneyi (sınıfın bir örneği) yaratacaktır NUMBER.add_two Şimdi nihayet yeni oluşturulan numaraya geçerek yöntemi gerçekten çağırmaya hazır.

Şimdi ilk kez, Ruby, basitçe yukarıdan aşağıya doğru giden varsayılan yürütme akışından sapmaya başlar. Bunun yerine, bir yöntem çağırdığımız için, Ruby şimdi daha önce yöntem için tanımladığımız yöntem gövdesine giriyor add_two: kontrol akışı şimdi 2.satıra atlıyor.

Bu anda argümanı olan bir metoda girdiğimiz için, Ruby ayrıca bir yerel değişken tanımlar number ve geçirilen nesneyi, sayıya 3 bu değişkene atar.

+Şimdi Ruby 2.satırı değerlendirmeye hazır. Değişkene atanan değer olan, number operatörünü kullandığımızı buluyor 3. Bunu yapmak için Ruby önce operatörün sağ tarafında bulunan, örneğimizde yine bir satı olan şeyi değerlendirir. NUMBER Bu nedenle Ruby, bu sefer değeri ile sayıyı (sınıfın bir örneği) yaratacaktır.

2 Ruby artık operatörü değerlendirmeye ve sayıya sayıyı eklemeye hazırdır 3. Bu işlem, olan yeni bir sayı (sınıfın bir örneği Number) döndürür 5.

Ruby yöntem gövdesinin sona erdiğini anlar ve bu nedenle, son değerlendirilen ifadenin dönüş değeri olduğundan add_two, dönüş değeriyle yöntemden döner 5.

Bu, Ruby’nin ikinci atlayışıdır:kontrol akışı satır 5’e geri döner.Ruby artık yöntem çağrısını değerlendirmeyi tamamlamıştır add_two(3) ve bu yöntem çağrısını nesneyi döndürmüştür 5.

puts Ruby, sonunda nesneyi geçen yöntemi çağırabilir ve 5 daha sonra yazdıracaktır.

Örnekler

[KİŞİYİ SELAMLAYIN](https://www.educative.io/courses/learn-ruby-from-scratch/mE0xABkW38O)

```ruby
# Start your code here 
def greet(name)
result = "Hello #{name}!"
return result  
end
```

[RASTGELE SELAMLAYIN](https://www.educative.io/courses/learn-ruby-from-scratch/mE0xABkW38O)

```ruby
# Start your code herege
def greet (name)
greetings = ["Hello", "Hi", "Ohai", "ZOMG"].shuffle
result = "#{greetings.first} #{name}!" 
return result
end
```

[MİLLERİ KİLOMETREYE DÖNÜŞTÜR](https://www.educative.io/courses/learn-ruby-from-scratch/RMlq00LqkOY)

```ruby
# Start your code here 
  def miles_to_kilometers(miles)
  result = miles * 1.609_34
  return result
  end
```

[ARTIK YILI KONTROL EDİN](https://www.educative.io/courses/learn-ruby-from-scratch/7nYzBD5gOxA)

```ruby
# Start your code here
  def leap_year?(year)
  result = (year % 400 == 0 or year % 100 != 0 and year % 4 == 0)
  return result
  end
```

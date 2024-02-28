# Savollar :

1. ### meta teglar vazifasi ?
2. ### pesudo class va pseudo element farqi?
3. ### mixin vs extend farqi ?
4. ### javascript data types ?
5. ### variables difference ?
6. ### Number methods 
7. ### Math object
8. ### String methods 
9. ### Undefined vs null ?
10. ### truthy , falthy ? 

<hr>

# Javoblar :

### 1 :

```

Meta teglar veb-saytlarda HTML kodida foydalaniladigan teglar hisoblanadi. Ularning vazifalari quyidagilardir:

1. Sahifa ma'lumotlari: Meta teglar veb-sahifalarning yoki veb-saytlarning ma'lumotlarini belgilaydi. Masalan, sahifa sarlavhasi (title), sahifa tavsifi (description), sahifa muallifi (author) kabi ma'lumotlar meta teglar orqali belgilanadi.

2. Qidiruv tizimlari uchun ma'lumotlar: Meta teglar qidiruv tizimlari (masalan, Google, Bing) kabi tizimlar uchun sahifalarning mazmuni va qiyosiy ma'lumotlarni ta'rifi uchun ishlatiladi. Bu, veb-saytni qidirish va tartiblashda muhim bo'lib, saytni qidiruv natijalarida chiqadigan ma'lumotlar uchun muhimdir.

3. Kod strukturasi optimizatsiyasi: Meta teglar HTML strukturasi va veb-saytning kodini optimallashtirish uchun ishlatiladi. Bu, brauzerlarga veb-saytni to'g'ri tushunish va qayta ishlashni osonlashtiradi.

4 .Ishga tushirish: Ba'zi meta teglar, masalan, <meta http-equiv="refresh" content="5;url=http://example.com/"> shaklida ishlatilgan holda, brauzerga biror muddatdan so'ng boshqa sahifaga otomatis ravishda o'tish buyrug'i berish uchun ishlatiladi.

5. Xususiy tomonlar uchun ma'lumotlar: Boshqa xususiy ma'lumotlar uchun ham meta teglar ishlatiladi, masalan, robots.txt fayli bilan birgalikda brauzerga veb-saytga kirish huquqini belgilovchi ma'lumotlar (meta tegi robots) saqlanadi.

Meta teglar sahifalarni brauzerlarga, qidiruv tizimlarga va boshqa avtomatlashtirilgan jarayonlarga ma'lumot berishda yordam beradi.
```

<br>
<hr>
<br>

### 2 :

```

Pesudo-class va pseudo-elementning farqi quyidagicha:

1. Pesudo-class: Pesudo-class, HTML elementlarga yo'l yo'naltirish berish uchun ishlatiladi va : belgisi bilan boshlanadi. Misol uchun, :hover, :active, :first-child kabi. Pesudo-classlar, elementning turini (masalan, hovli, bosqich, oddiy o'zgaruvchi) yoki foydalanuvchining amalini (masalan, turga olib borish, ustuvor joyga olib borish) belgilaydi. Pesudo-classlar, HTML elementlarga dinamik ravishda yo'l yo'naltirish berishga yordam beradi.

2. Pesudo-element: Pesudo-element, HTML elementning bir qismi, ya'ni elementning ma'lum bir qismi uchun xususiyatlarni belgilash uchun ishlatiladi va :: belgisi bilan boshlanadi. Misol uchun, ::before, ::after, ::first-line kabi. Pesudo-elementlar, HTML elementlarining qismlari sifatida amal qiladi va yangi HTML elementini yaratmaydi, balki mavjud elementning bitta qismiga stil qo'shadi. Misol uchun, ::before pesudo-elementi yordamida bir elementning oldida yangi ma'tn qo'shish mumkin.

Asosiy farq, pesudo-classlar elementning o'zini yo'l yo'naltirishda ishlatiladi, pesudo-elementlar esa elementning bir qismiga stil qo'shishda ishlatiladi.
```

<br>
<hr>
<br>

### 3 :

```
Mixin va extend Sass dasturlash tillarida ushbu ixtiyoriy funksiyalarni birlashtirish uchun ishlatiladi, lekin ularga farq mavjud:

Mixin: Mixin, ko'p marta ishlatiladigan ko'p qatorli kod bloklarini birlashtirish uchun ishlatiladi. Mixin, stil qo'llash uchun funksiya sifatida ishlaydi va bir nechta stil qo'shimlarni birlashtirishda va ularga o'zgaruvchilar orqali o'zgartirishlar kiritishda foydalaniladi. Mixin funksiyasi, istalgan CSS stilini generatsiyalaydi. Misol uchun, sizning saytingizning butun sahifasiga bir xil rang shema berishingiz kerak bo'lsa, bu ranglarni bitta mixin ichida qo'llab-quvvatlash mumkin. Mixinlar, .scss yoki .sass fayllarida yaratiladi va .sass sintaksisida funksiya sifatida chaqiriladi.
```
### Misol :
```
@mixin rounded-corners($radius) {
  border-radius: $radius;
}

.button {
  @include rounded-corners(5px);
  background-color: blue;
}
```

```
Extend: Extend, bir yoki bir nechta stil qo'shimlarini (klasslarni) boshqaruvchi klassga asoslab ishlaydi. Bu, bir klassning barcha xususiyatlarini boshqa bir klassga o'tkazishni ta'minlaydi. Extend, klasslarning o'zidan boshqa klasslarga o'tkazilishiga imkoniyat beradi. Bunga klass qo'llab-quvvatlash (@extend) va turli klasslar orasida ishonch yaratish (%placeholder) imkoniyati kiritilgan. Extend, foydalanilgan klasslarning barcha xususiyatlarini boshqalariga o'tkazadi, shuning uchun kodni optimallashtirish uchun juda samarali bo'ladi. Extend %placeholder bilan aniqlanadi va .scss fayllarida yaratiladi.
```

### Misol :
```
%rounded-corners {
  border-radius: 5px;
}

.button {
  @extend %rounded-corners;
  background-color: blue;
}
```

```
Asosiy farq, mixinlar faktik narsalarni generatsiyalash uchun ishlatiladi, extend esa mavjud narsalarni boshqa narsalarga o'tkazish uchun ishlatiladi. Mixinlar funksiya sifatida ishlaydi va stilni generatsiyalaydi, extend esa klasslarni birlashtiradi va ularga o'zlarini o'tkazadi.
```

<br>
<hr>
<br>

### 4 :

```

JavaScriptda quyidagi ma'lumot turlari (data types) mavjud:

Primitive Types (Oddiy tur):

1. String: Matnlar (qatorlar).
2. Number: Sonlar.
3. Boolean: Mantiqiy qiymatlar, ya'ni true va false.
4. Null: Bo'sh qiymat (hech narsa yo'q).
5. Undefined: O'zgaruvchi e'tiborsiz (hali qiymat olinmagan).
6. Symbol: ES6 (ECMAScript 2015) dan boshlab qo'shilgan, unikal belgilar.

 - Composite Types (Qo'shimcha tur):

1. Object: Kerakli malumotlarni yig'ish uchun ob'ekt.
2. Array: Ma'lumotlar to'plami, ko'p elementlardan iborat.

 -Special Types (Maxsus tur):

1. Function: Funksiyalar (o'zgaruvchilarni qabul qilish, amallarni bajarish).
2. Date: Sanalar va vaqtlar.
3. RegExp: Regulyar ifodalar (matnlar ustida patternlar izlash uchun).
4. Error: Xato ob'ektlari.

JavaScript, dinamik tildir, ya'ni o'zgaruvchilarning turini avtomatik ravishda aniqlab, mos ravishda ko'rsatishga urinadi. Bu ma'noda, o'zgaruvchining turini taxmin qilish uchun o'zgaruvchilarni o'zlarini bajarish sharti emas.
```

<br>
<hr>
<br>

### 5 :

```
JavaScriptda o'zgaruvchilar (variables) alohida qiymatlarni saqlash uchun ishlatiladi. Ularning turli turlari va farqlari mavjud:

var, let va const:

var ES5 dan oldin, let va const esa ES6 (ECMAScript 2015) bilan kiritilgan. Ularning farqlari:
var: Funksiya miqyosida o'zgaruvchilarni e'lon qiladi va barcha funktsiyalarda ko'rinadi. var o'zgaruvchilari hoisting qilinadi.
let: Block-scope ni qo'llaydi. Bunaqangi o'zgaruvchi faqatgina yaratilgan block ichida (masalan, if, for, while bloklari) mavjud bo'ladi.
const: let bilan bir xil bo'lsa, lekin o'zgaruvchi o'zgartirilmaydi (immutable). const bilan yaratilgan o'zgaruvchilarga boshlang'ich qiymat berilishi shart.
Primitive vs. Reference Types:

Primitive (Oddiy) Turlar: String, Number, Boolean, Undefined, Null, Symbol. Bu turdagi o'zgaruvchilar qiymatni o'zida saqlaydi. Agar bir o'zgaruvchidan boshqa o'zgaruvchiga qiymat o'tkazilsa, o'zgaruvchining asl qiymati ko'chiriladi.

Reference (Uzviy) Turlar: Array, Object, Function. Bu turdagi o'zgaruvchilar ob'ektlarni ko'rsatish (reference)ni saqlaydi. Bu ob'ektlar ro'yxatlar, ob'ekt haqida ma'lumotlar, funksiyalar kabi bo'lishi mumkin. Agar bir reference o'zgaruvchidan boshqa o'zgaruvchiga qiymat o'tkazilsa, asl reference o'zgartirilmaydi, balki yangi o'zgaruvchi asl ob'ektni ko'rsatadi.
Scope va Lifetime:

Scope (Hudud): O'zgaruvchining aniqlanish joyi (mavjudligi). var funksiya miqyosida o'zgaruvchini o'rnatsa-da, let va const block-scope da o'zgaruvchilar o'rnatsa.

Lifetime (Muddat): O'zgaruvchining mavjud bo'lishi vaqti. Agar o'zgaruvchi bir funksiya ichida e'lon qilinsa, uni faqat shu funksiya ichida ishlatishingiz mumkin. Agar global o'zgaruvchidan boshqa joyda e'lon qilinsa, uni dastur bo'lguncha ishlatishingiz mumkin.

JavaScriptda o'zgaruvchilar o'z tur va muhitiga ko'ra turli xususiyatlarga ega bo'ladi. Bu xususiyatlar, o'zgaruvchi turiga va uning qanday qilib e'lon qilinishiga bog'liqdir.
```

<br>
<hr>
<br>

### 6 :

```

```

<br>
<hr>
<br>

### 7 :

```

```

<br>
<hr>
<br>

### 8 :

```

```

<br>
<hr>
<br>

### 9 :

```

```

<br>
<hr>
<br>

### 10 :

```

```

<br>
<hr>
<br>



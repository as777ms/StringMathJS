# JavaScript String & Math Methods
>There may come various instances where we need to manipulate strings in it.`krch dar zindagi misol vaqte ki wumo bo js kro mekuned yagon zadacha meoyad ki wumo dar in xolat bo string kor kunad yane vairon manipulirovat kardanawro yod gired in kor xele duwvor ast ba vositai for (baroi xamin methpdxo baromadand to in ki kori moro osoon kunand)`


**_So, let’s discuss the basic string methods in JavaScript._**

 * 1) Length Method
* 2) CharAt Method
* 3) EndsWith Method
* 4) Includes Method
* 5) IndexOf Method
* 6) Match Method
* 7) Repeat Method
* 8) Replace Method
* 9) Slice Method
* 10) Split Method
* 11) StartsWith Method
* 12) Substr Method
* 13) Substring Method
* 14) ToLowerCase Method
* 15) ToUpperCase Method
>Here, I have mentioned 15 string methods that are commonly used in javascript. Let’s discuss them in detail. i lenghta return mekna dazhe spaceoi xoliwa xisob mekna

# 1) Length Method
>methodi length ro baroi xisob kardani masofai string istifoda mebarand
⬇️ sintaxisaw
```js
let string.length;
```
```js
let str = "Hello Cybrosys";
let str_len = str.length;
console.log("length", str_len);//length 14
```

# 2)CharAt method
>methidi charAt da mo indexi darkori mona metem mebrora xarfa (index ai 0 sar mewava) baroi giriftani 1 xarf mo 0 metem dar daruni parametroi charAt
⬇️ sintaxsisw
```js
string_variable.charAt(‘index’);
```
```js
let str = "Hello Cybrosys";
let char_at = str.charAt(6);
console.log(char_at); //C chiba C baroi on ki spaceora xisob kadai znachit
```

# 3) EndsWith Method
>methodi endWith returnw true yo false ai aga biyova oxiraki xamu text ba xamu parametri doxil kadagii mo tugri bgira
⬇️ syntexisw
```js
string_variable.endsWith(‘characters’);
```
```js
let str = "Hello Cybrosys";
let is_last = str.endsWith('sys');
console.log(is_last);//true
```

```js
let str = "Hello Cybrosys";
let is_last = str.endsWith('C');
console.log(is_last);//false meta baroi on ki oxiri i text C nest (znachit rangi includes nest)
```

# 4) Includes Method
>i true you false mebrora mekova agar youft true aga nayoft false ida rangi unau torgi farq nadora chi i da oxirai chi da mobain chi da aval agar xamu chi da text bowa true false wa mebrora
⬇️ syntexisw
```js
string_variable.includes(‘characters’);
```
```js
let  str = "Hello Cybrosys";
let is_incl = str.includes('sys');
console.log(is_incl);//true
```

```js
var str = "Hello Cybrosys";
var is_incl = str.includes('xyz');
console.log(is_incl);//false meta baroi ki itari chi nest
```

# 5) IndexOf Method
>IndexOf method indexi xamu xarfi da parametr mondagii mora mebrora aga nayoft -1 mebrora
⬇️ syntexisw
```js
string_variable.indexOf(‘characters’);
```
```js
var str = "Hello Cybrosys";
var index_char = str.indexOf('sys');
console.log(index_char);//11 meta baroi ki xarfi avalwa mebina agane boyad 13 bta ku
```
# 6) Match Method
>i masiv mebrovardai indexw qati xamu (chze ki mo da parametr drovardem indexwa) bad bo input: "xamu texta polni xcha" bad bo groups: undefined mebrovardai aga nayova null mebrora

```js
string_variable.match(‘expression’);
```
```js
let str = "Hello Cybrosys";
let match_expr = str.match("sys");
console.log(match_expr);//[ 'sys', index: 11, input: 'Hello Cybrosys', groups: undefined ]
```


# 7) Repeat Method
>ira megem ki chanbor repeat kna i takror mekna xamu texta yo xarfa
```js
string_variable.repeat(‘count’);
```
```js
var str = "Hello Cybrosys";
var repeat_expr = str.repeat(3);
console.log(repeat_expr);//Hello CybrosysHello CybrosysHello Cybrosys
```

# 8) Replace Method
>i chira ba chi aliw knak methodai 2 parametr megira chira ba chi aliw kna (kadom xarfa yo kalimara ba chi) aga nayoft xamu chzi aliw mekadagira xdi stringa return mekna

```js
str = "Hello Cybrosys";
let replace_expr = str.replace('Hello', "Anisa");
console.log(replace_expr);//Anisa Cybrosys
```
 
# 9) Slice Method
>ida 2 ta argument roi meknem start end ai kujo sar wava to kjo brava (ba indexi xarfo metem) i -0 ram qabul mekna rangi substringai prosto u - 0 qabul namekna aga 1 argument roi knem ai sarwavi to ixiri stringa mebrora
```js
let str = "Hello Cybrosys";
let slice_expr = str.slice('6', '11');
console.log(slice_expr);//Cybro
```

# 10) Split Method
> i stringa mesaiv mekna vobasta ba on ki mo chxeli bgemw aga ("") xamai xarfora judo mekna aga (",") cherez vergul judowon mekna bo ya chii diga i space oram judo mekna 
```js
var str = "Hello Cybrosys";
var split_expr = str.split('');
console.log(split_expr);//['H', 'e', 'l', 'l','o', ' ', 'C', 'y','b', 'r', 'o', 's','y', 's']
```

# 11) StartsWith Method
>i true you false mebrora agar da sarwavii string xamu chizi roi kadagii mo bowa agar nabowa false i indexam kak 2 parametr megira indexwa yoft true false mega

```js
var str = "Hello Cybrosys";
var start_expr = str.startsWith("He");
console.log(start_expr);//true
```

```js
var str = "Hello Cybrosys";
var start_expr = str.startsWith("Cy", 6);
console.log(start_expr);//ijada true meta chixele ki guftem mesanja indexw tugriay ba xamu
```

# 12) Substring Method
>chi xele ki guftem i rangi slice ai tolko u -minusa qabul mekna i ne start end dora
```js
var str = "Hello Cybrosys";
var substring_expr = str.substring(13, 5);
console.log(substring_expr);//Cybrosy
```


# 13) ToLowerCase Method
>i past mekna vesi xamu xarfora
```js
var str = "Hello Cybrosys";
var toLowerCase_expr = str.toLowerCase();
console.log(toLowerCase_expr);//hello cybrosys
```

# 14) ToUpperCase Method
>i baland mekna vesi xamu xarfora
```js
var str = "Hello Cybrosys";
var toUpperCase_expr = str.toUpperCase();
console.log(toUpperCase_expr);//HELLO CYBROSYS
```


### Math Methods
# 1) Math.abs()
>i minusara + mekna
```js
Math.abs(-1); // 1
```
# 2) Math.floor()
>i xamu adad azdax doram bowa xamu adada niwon meta to xdi adada kalonw nawava maqsad azdaxdorakwa megira
```js
console.log(Math.floor(5.95));
// Expected output: 5
```
# 3) Math.min()
>i xurdtarina da baini xamu adad mebrora
```js
console.log(Math.min(1, 3, 2));
// Expected output: 1
```

# 4) Math.max()
>i kalontarina da baini xamu adad mebrora
```js
console.log(Math.max(1, 3, 2));
// Expected output: 3
```

# 5) Math.pow()
>i darajai xamu adata mebrora 2 parametr megira 1 kadom adad 2 darajaw
```js
console.log(Math.pow(7, 3));
// Expected output: 343
```

# 6) Math.random()
> i randomno mebrora ai 0 to 0 az mlrd baroi ki moda adadi darkorimona bubrora darkorai ki ura ba i zar knm
```js
let a=10
let a2=(Math.floor(Math.random()*10))
console.log(a2);//it will return everything till 10
```

# 7) Math.round()
>ida xami azdax 1 ki wid uzhe kalon mexisoba raqama
```js
console.log(Math.round(0.9));
// Expected output: 1
```

# vi-hafta-odev

- JavaScript'te nesne(object) örnekleri yaratarak örnekler içerisinde metodlarla birlikte kullanmaya çalışınız.
ANSWERS:
1.
<!DOCTYPE html>
<html>
   <body>
      <p id="demo"></p>

      <script>
         // Create an object:
         var person = {
           firstName: "John",
           lastName : "Doe",
           id     : 5566,
           fullName : function() {
             return this.firstName + " " + this.lastName;
           }
         };
        // Display data from the object:
        document.getElementById("demo").innerHTML = person.fullName;
      </script>
   </body>
</html>

- 'return' ve 'console.log' arasındaki farkı açıklayınız. Örneklerle destekleyiniz. 
ANSWERS:
1. Bazen fonksiyonun geriye göndereceği değeri ekrana çıktı vermek yerine bir değişken ya da başka bir fonksiyonda daha sonra kullanmamız gerekebilir. Bu gibi durumlarda fonksiyon gövdesinde return ifadesini kullanırız.
2.  function addition(sayi1,sayi2){
        return (sayi1+sayi2);
    }
    var add = addition(1,2);   //add değişkenine 1+2 değerini fonksiyon kullanarak atadık.

- JavaScript'te primitive types ve reference types kavramlarını araştırınız. Bu sınıflandırmalara dahil olan türleri sıralayınız.
ANSWERS:
1. Boolean, Null, Undefined, Number, BigInt, String, Symbol, Object
2. If the value is a primitive value, when you access the variable, you manipulate the actual value stored in that variable. In other words, the variable that stores a primitive value is accessed by value.

   Unlike a primitive value, when you manipulate an object, you work on the reference of that object, rather than the actual object. It means a variable that stores an object is accessed by reference.

- 'for in' ve 'for of' döngülerini açıklayınız ve örneklerle destekleyiniz.
ANSWERS:
1. If counters/indexes are needed while accessing an array or indexes related logical stuff are there it is better to go ahead with for loop.
2. If there is a need to access properties/keys regardless of the order for-in will help.
3. If you just need to iterate through data items of an iterable(also if you need to apply some changes maybe) for-of is an obvious choice.

- 'for' ve 'while' döngüleri ile ilgili örnekler yapınız.
ANSWERS:
1. For: Loops can execute a block of code a number of times.
    for (i = 0; i < cars.length; i++) {
      text += cars[i] + "<br>";
    }
2. While: Loops can execute a block of code as long as a specified condition is true.
    while (i < 10) {
      text += "The number is " + i;
        i++;
    }

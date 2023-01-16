# -LT-22_Nullish_Coalesting_Operator

`Nullish coalescing operator (??)` adalah operator baru dalam JavaScript yang digunakan untuk mengevaluasi ekspresi dengan nilai default jika ekspresi pertama bernilai null atau undefined. Operator ini memiliki dua bagian: ekspresi pertama dan ekspresi kedua. Operator ini disajikan dalam bentuk:

    ekspresi1 ?? ekspresi2;

Jika ekspresi1 bernilai null atau undefined, ekspresi2 akan dievaluasi dan dihasilkan, jika tidak, ekspresi1 akan dihasilkan. Contoh :

    let name = null;
    let myName = name ?? "John";
    console.log(myName); // "John"

Dalam contoh di atas, operator nullish coalescing digunakan untuk memberikan nilai default "John" jika variabel name bernilai null. Sebelum adanya operator ini, untuk menentukan nilai default dari sebuah variabel, biasa menggunakan operator logika OR (||) yang memiliki beberapa masalah dalam kasus seperti 0, empty string, atau false.

    let name = "";
    let myName = name || "John";
    console.log(myName); // "" 

Secara keseluruhan, Nullish coalescing operator adalah operator baru dalam javascript yang digunakan untuk mengevaluasi ekspresi dengan nilai default jika ekspresi pertama bernilai null atau undefined dan memberikan solusi dalam kasus yang tidak dapat diatasi dengan operator OR (||) sebelumnya.

Selain itu, operator nullish coalescing juga dapat digunakan dalam kombinasi dengan operator lain untuk menulis ekspresi yang lebih kompleks. Contohnya:

    let name = "";
    let myName = name ?? (age > 18 ? "Adult" : "Child") ;
    console.log(myName); // "Child"

Dalam contoh di atas, operator nullish coalescing digunakan dalam kombinasi dengan operator ternary untuk menentukan nilai dari myName berdasarkan nilai dari name dan age. Jika name bernilai null atau undefined, maka akan di eksekusi operator ternary didalamnya dan memberikan nilai dari myName.

Secara umum, operator nullish coalescing dapat digunakan untuk menulis kode yang lebih singkat dan mudah dibaca, namun perlu diingat bahwa ekspresi yang terlalu kompleks dapat membuat kode menjadi sulit dibaca dan dipahami. Oleh karena itu, selalu disarankan untuk menjaga kode Anda sederhana dan jelas sambil menggunakan operator nullish coalescing.

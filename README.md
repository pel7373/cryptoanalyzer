# Cryptoanalyzer / Криптоаналізатор

   Шифрування/розшифрування відбувається на основі алфавіту: "ABCDEFGHIJKLMNOPQRSTUVXYZabcdefghijklmnopqrstuvxyz.,\":-!? "

1. Шифрування: програма шифрує текст, використовуючи заданий криптографічний ключ.

   В графічному інтерфейсі треба вказати: 
     а) ім'я текстового файлу з вхідним текстом; 
     б) ключ - на скільки символів в алфавіті зсовується текст; 
     в) ім'я вихідного файла.
  
   В результаті створюється вихідний зашифрований текстовий файл. 
   Якщо в тексті зустрічається інший символ (який не входить до алфавіту) - він не обробляється.

2. Розшифрування: програма розшифровує текст, використовуючи заданий криптографічний ключ.

   В графічному інтерфейсі треба вказати: 
     а) ім'я текстового файлу з вхідним текстом; 
     б) ключ - на скільки символів в алфавіті зсовується текст; 
     в) ім'я вихідного файла.

   В результаті створюється вихідний розшифрований текстовий файл. 

3. Криптоаналіз методом brute force: програма зламує зашифрований текст. 

   Зламування відбувається перебором різних ключів (від 0 до довжини алфавіту) і для розшифрованого тексту з кожним ключем підраховується кількість співпадінь зі словником. 
   Правильний ключ - це ключ, при якому відбулась найбільша кількість співпадінь.
   При цьому використовується словник, який зчитується з файла.

   В графічному інтерфейсі треба вказати: 
     а) ім'я текстового файлу з вхідним текстом; 
     б) ім'я вихідного файла;
     в) ім'я файла словника.

   В результаті:
     а) на екран виводиться повідомлення, який ключ підібрано;
     б) створюється вихідний розшифрований текстовий файл. 

4. Криптоаналіз методом статистичного аналізу.

   Завантажуємо додатковий файл із текстом, бажано — того самого автора і тієї самої стилістики.
   Програма складає статистику входження символів у закодований текст і додатковий файл із текстом.
   Підраховуємо для вісьми найвживаніших літер у вхідному і додатковому тексті - відстань між цими буквами у алфавіті.
   Тобто вираховуємо різницю між першою найвживанішою літерою у вхідному і у додатковому тексті, між другою..., і так до восьмої. 
   Зрозуміло, що значення різниці для цих пар літер (від першої і до восьмої) може бути різним. 
   Тому підраховуємо, яка різниця зустрічається частіше - це і буде наш ключ, з яким ми будемо разкодовувати вхідний текст.

   В графічному інтерфейсі треба вказати: 
     а) ім'я текстового файлу з вхідним текстом; 
     б) ім'я вихідного файла;
     в) ім'я файла з додатковим текстом.

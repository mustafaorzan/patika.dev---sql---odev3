# patika.dev---sql---odev3
https://app.patika.dev/cataldirect

1 - country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.

CEVAP: 

    SELECT * FROM country WHERE country  LIKE 'A%a'
    
2 - country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.

CEVAP: 

    SELECT * FROM country WHERE country  LIKE '______%n'
    
3 - film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.

CEVAP: 

    SELECT title FROM film WHERE title ILIKE '%T%T%T%T'
        
4 - film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.

CEVAP:

    SELECT * FROM film WHERE title LIKE 'C%' and length>90 and rental_rate=2.99

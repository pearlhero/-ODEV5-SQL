# -ODEV5-SQL
dvdrental sorgu senaryoları çözümleri
Sorgu 1- film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
Çözüm 1- SELECT title FROM film
WHERE title ILIKE '%n'
ORDER BY length DESC
LIMIT 5;
<img width="533" alt="Ekran Resmi 2023-03-03 14 52 54" src="https://user-images.githubusercontent.com/116847744/222714203-91662393-7805-4da9-b529-3ffdc153f57c.png">

Sorgu 2- film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
Çözüm 2- SELECT title FROM film
WHERE title ILIKE '%n'
ORDER BY length ASC
OFFSET 5
LIMIT 5;
<img width="578" alt="Ekran Resmi 2023-03-03 14 59 26" src="https://user-images.githubusercontent.com/116847744/222714982-7194d195-4931-47e2-8d98-619c94763fb8.png">

Sorgu 3- customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.
Çözüm 3- SELECT last_name, store_id FROM customer
WHERE store_id = 1
ORDER BY last_name DESC
LIMIT 4;
<img width="547" alt="Ekran Resmi 2023-03-03 15 04 50" src="https://user-images.githubusercontent.com/116847744/222716027-d2108126-85cf-4686-bd5f-97150589ddad.png">



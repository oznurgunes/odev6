1)film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?<br><code>
  select avg(rental_rate) from film;</code><br>
2)film tablosunda bulunan filmlerden kaçtanesi 'C' karekteri ile başlar?<br><code>
  select COUNT(*) from film
where title like 'C%';</code><br>
3)film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?<br><code>
  select max(length) from film
where rental_rate=0.99;</code><br>
4)film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?<br><code>
  select count(distinct replacement_cost) from film
where length>150;


## Aşağıdaki sorgu senaryolarını ***dvdrental*** örnek veri tabanı üzerinden gerçekleştiriniz.

1) **test** veritabanınızda **employee** isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

```sql
create table employee (
	id integer,
	name varchar(50),
	birthday date,
	email varchar(100)
	);
 ```

2) Oluşturduğumuz **employee** tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```sql 
```

3) Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

```sql 
update employee
set name = 'Emily Gwelyn'
where id = 7;
```
```sql 
update employee
set birthday = '1952-02-22'
where name = 'Bianca Mourge';
```
```sql 
update employee
set email = 'veronika@kodluyoruz.com.tr'
where id = 14;
```
```sql 
update employee
set name = 'Frida Kahlo',
	birthday = '1991-10-11'
where id = 43;
```
```sql 
update employee
set birthday = '1941-10-11',
	email = 'frida@lambda.tx'
where id = 43;
```

4) Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

```sql 
delete from employee
where id = 31;
```
```sql 
delete from employee
where name = 'Nico Dunk';
```
```sql 
delete from employee
where name like  '%n%';
```
```sql 
delete from employee
where birthday < '1960-01-01';
```
```sql 
delete from employee
where email like '%.com';
```

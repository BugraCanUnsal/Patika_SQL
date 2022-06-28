# SQL - ODEV8

Merhabalar,

1. test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
2. Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

Kolay Gelsin.

----
```
CREATE TABLE employee (
    id INTEGER PRIMARY KEY,
    name VARCHAR(50),
    birthday DATE,
    email VARCHAR(100)    
);
````
---
```
insert into employee (id, name, birthday, email) values (1, 'Leslie', '1993-03-09', 'lfuster0@google.com.br');
insert into employee (id, name, birthday, email) values (2, 'Orran', '2005-05-29', 'okingham1@zimbio.com');
insert into employee (id, name, birthday, email) values (3, 'Debor', '2022-05-07', 'djanuszewski2@amazon.co.jp');
insert into employee (id, name, birthday, email) values (4, 'Rina', '1991-08-26', 'rrobilart3@blinklist.com');
insert into employee (id, name, birthday, email) values (5, 'Christoffer', '1997-04-24', 'cnorres4@w3.org');
insert into employee (id, name, birthday, email) values (6, 'Allie', '1993-06-13', 'acoddington5@flavors.me');
insert into employee (id, name, birthday, email) values (7, 'Linell', '2007-03-19', 'lmcgarrity6@feedburner.com');
insert into employee (id, name, birthday, email) values (8, 'Domenico', '2020-02-22', 'dtredger7@answers.com');
insert into employee (id, name, birthday, email) values (9, 'Chaim', '2015-06-07', 'cpotteridge8@quantcast.com');
insert into employee (id, name, birthday, email) values (10, 'Nikolai', '2004-01-16', 'nyes9@about.com');
insert into employee (id, name, birthday, email) values (11, 'Ilysa', '2001-07-24', 'ibinga@about.me');
insert into employee (id, name, birthday, email) values (12, 'Pepito', '2016-09-02', 'pmcchesneyb@jigsy.com');
insert into employee (id, name, birthday, email) values (13, 'Luisa', '1992-08-05', 'lhabletc@accuweather.com');
insert into employee (id, name, birthday, email) values (14, 'Hermina', '2020-11-30', 'hchipmand@house.gov');
insert into employee (id, name, birthday, email) values (15, 'Bevon', '1994-06-11', 'bwillowaye@odnoklassniki.ru');
insert into employee (id, name, birthday, email) values (16, 'Merralee', '1998-01-27', 'mnormanf@nymag.com');
insert into employee (id, name, birthday, email) values (17, 'Isac', '2016-04-10', 'ibilbyg@npr.org');
insert into employee (id, name, birthday, email) values (18, 'Claiborn', '1993-05-27', 'clevickh@nytimes.com');
insert into employee (id, name, birthday, email) values (19, 'Tasia', '2015-07-05', 'tgoodinsoni@w3.org');
insert into employee (id, name, birthday, email) values (20, 'Germayne', '1990-10-09', 'gtethacotj@vistaprint.com');
insert into employee (id, name, birthday, email) values (21, 'Dacie', '1999-09-13', 'dmertonk@so-net.ne.jp');
insert into employee (id, name, birthday, email) values (22, 'Opal', '1991-03-18', 'oshanksl@zimbio.com');
insert into employee (id, name, birthday, email) values (23, 'Eduardo', '1994-07-31', 'escurrerm@rakuten.co.jp');
insert into employee (id, name, birthday, email) values (24, 'Bobinette', '2009-09-03', 'bmcgown@hp.com');
insert into employee (id, name, birthday, email) values (25, 'Shena', '1998-03-02', 'spickupo@netlog.com');
insert into employee (id, name, birthday, email) values (26, 'Rozalie', '2009-08-08', 'rtilmouthp@qq.com');
insert into employee (id, name, birthday, email) values (27, 'Perceval', '1997-02-09', 'pweightq@google.com.br');
insert into employee (id, name, birthday, email) values (28, 'Jasmin', '2016-10-15', 'jfeldharkerr@merriam-webster.com');
insert into employee (id, name, birthday, email) values (29, 'Esdras', '1992-12-20', 'einkpins@tamu.edu');
insert into employee (id, name, birthday, email) values (30, 'Shelden', '1998-07-15', 'swissont@yellowpages.com');
insert into employee (id, name, birthday, email) values (31, 'Byrle', '2001-08-24', 'bminkinu@huffingtonpost.com');
insert into employee (id, name, birthday, email) values (32, 'Paco', '2017-12-01', 'pnaptinv@opensource.org');
insert into employee (id, name, birthday, email) values (33, 'Kacie', '2003-05-14', 'kdanilovicw@craigslist.org');
insert into employee (id, name, birthday, email) values (34, 'Greer', '2020-02-23', 'gallportx@tuttocitta.it');
insert into employee (id, name, birthday, email) values (35, 'Dore', '1999-01-23', 'dtattertony@nba.com');
insert into employee (id, name, birthday, email) values (36, 'Allan', '2006-01-05', 'ayearnz@youtu.be');
insert into employee (id, name, birthday, email) values (37, 'Shirline', '2012-08-16', 'spaintain10@prnewswire.com');
insert into employee (id, name, birthday, email) values (38, 'Hort', '2017-04-25', 'hholberry11@odnoklassniki.ru');
insert into employee (id, name, birthday, email) values (39, 'Aindrea', '1993-12-02', 'agatherer12@stumbleupon.com');
insert into employee (id, name, birthday, email) values (40, 'Luci', '2011-11-27', 'lmcinulty13@wiley.com');
insert into employee (id, name, birthday, email) values (41, 'Tiphany', '2002-09-18', 'tgrewes14@flickr.com');
insert into employee (id, name, birthday, email) values (42, 'Arielle', '1992-10-08', 'abodker15@jigsy.com');
insert into employee (id, name, birthday, email) values (43, 'Cleavland', '2008-06-11', 'cprovest16@infoseek.co.jp');
insert into employee (id, name, birthday, email) values (44, 'Earl', '2000-07-05', 'etortis17@goo.gl');
insert into employee (id, name, birthday, email) values (45, 'Briggs', '2016-07-29', 'bcunnington18@go.com');
insert into employee (id, name, birthday, email) values (46, 'Chris', '2015-07-08', 'ctrevascus19@chronoengine.com');
insert into employee (id, name, birthday, email) values (47, 'Gloria', '2009-03-07', 'gtunaclift1a@privacy.gov.au');
insert into employee (id, name, birthday, email) values (48, 'Abelard', '1994-03-15', 'adumbrall1b@chron.com');
insert into employee (id, name, birthday, email) values (49, 'Dwain', '1996-09-15', 'dsarge1c@blogtalkradio.com');
insert into employee (id, name, birthday, email) values (50, 'Lynett', '2014-04-14', 'ljeanesson1d@cpanel.net');
```
----
```
UPDATE employee
SET name = 'Ali',
    birthday = '1993-12-20',
    email = 'aliali@aliali.com'
WHERE id = 1;

UPDATE employee
SET id = 51,
    birthday = '1993-12-20',
    email = 'aliali@aliali.com'
WHERE name = 'Lazar';

UPDATE employee
SET id = 52,
    name = 'Veli',
    email = 'veliveli@veliveli.com'
WHERE birthday = '1993-03-02';

UPDATE employee
SET id = 53,
    name = 'Ali',
    birthday = '1993-12-20'
WHERE email = 'rventham1b@addtoany.com';

UPDATE employee
SET name = 'Mahmut',
    birthday = '1993-12-20',
    email = 'mahmut@mahmut.com'
WHERE id = 5;
```
---
```
DELETE FROM employee WHERE id = 53;

DELETE FROM employee WHERE name = 'Ali';

DELETE FROM employee WHERE birthday = '1993-12-20';

DELETE FROM employee WHERE email = 'veliveli@veliveli.com';

DELETE FROM employee WHERE id = 51;
```
# HackerRank SQL

<p align="center">
  <img src="https://img.shields.io/badge/HackerRank-00EA64?style=flat&logo=hackerrank&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-F80000?style=flat&logo=oracle&logoColor=white"/>
  <img src="http://img.shields.io/static/v1?label=STATUS&message=Em Andamento&color=yellow&style=flat"/>
</p>

 <p align="center"><img src="https://github.com/almeidastor/imgsforreadme/blob/main/rackerankchal/icon.png"></p>

<p align="justify">
Resoluções do desafio Hacker Rank SQL/2023
</p>

### Sumário
🔹 [Desafio 01: Revising the Select Query I](#revising-the-select-query-i) 

🔹 [Desafio 02: Revising the Select Query II](#revising-the-select-query-ii)

🔹 [Desafio 03: Select All](#select-all)

🔹 [Desafio 04: Select By ID](#select-by-id)

🔹 [Desafio 05: Japanese Cities Attributes](#japanese-cities-attributes)

🔹 [Desafio 06: Japanese Cities Names](#japanese-cities-names)

🔹 [Desafio 08: Weather Observation Station 1](#weather-observation-station-1)

🔹 [Desafio 09: Weather Observation Station 3](#weather-observation-station-3)

🔹 [Desafio 10: Weather Observation Station 4](#weather-observation-station-4)

🔹 [Desafio 11: Weather Observation Station 5](#weather-observation-station-5)

🔹 [Desafio 12: Weather Observation Station 6](#weather-observation-station-6)

🔹 [Desafio 13: Weather Observation Station 7](#weather-observation-station-7)

🔹 [Desafio 13: Weather Observation Station 8](#weather-observation-station-8)

🔹 [Desafio 14: Weather Observation Station 9](#weather-observation-station-9)

🔹 [Desafio 15: Weather Observation Station 10](#weather-observation-station-10)

🔹 [Desafio 16: Weather Observation Station 11](#weather-observation-station-11)

🔹 [Desafio 17: Weather Observation Station 12](#weather-observation-station-12)

🔹 [Desafio 18: Higher Than 75 Marks](#higher-than-75-marks)

🔹 [Desafio 19: Employee Names](#employee-names)

🔹 [Desafio 20: Employee Salaries](#employee-salaries)

🔹 [TABELAS DE REFERENCIA](#tabelas-referencia)




## Revising the Select Query I
Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA. 
The CITY table is described as follows:

(<a href="#tabref1">Tabela Referencia 1</a>)


* Resolução: Select * from CITY where POPULATION > 100000 and COUNTRYCODE = "USA";



## Revising the Select Query II
Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

The CITY table is described as follows: 

(<a href="#tabref1">Tabela Referencia 1</a>)

* Resolução: Select * from CITY;


## Select By ID
Query all columns for a city in CITY with the ID 1661.

The CITY table is described as follows: 

(<a href="#tabref1">Tabela Referencia 1</a>)

* Resolução: Select * from CITY where ID = 1661;



## Japanese Cities Attributes
Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.

The CITY table is described as follows: 

(<a href="#tabref1">Tabela Referencia 1</a>)

* Resolução: Select * from CITY where COUNTRYCODE = "JPN";


## Japanese Cities Names
Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.
The CITY table is described as follows: 

(<a href="#tabref1">Tabela Referencia 1</a>)

* Resolução: Select NAME from CITY where COUNTRYCODE = "JPN";


## Weather Observation Station 1
Query a list of CITY and STATE from the STATION table.
The STATION table is described as follows: 

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: Select CITY, STATE From STATION;


## Weather Observation Station 3
Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.
The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: SELECT Distinct CITY From STATION Where MOD(ID,2)=0 Order By CITY asc; 

## Weather Observation Station 4
Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.
The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: Select Count(CITY) - Count(Distinct CITY) From STATION;


## Weather Observation Station 5
Query the two cities in STATION with the shortest and longest CITY names, as well as their respective lengths (i.e.: number of characters in the name). If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically.
The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: select CITY,LENGTH(CITY) from STATION order by Length(CITY) asc, CITY limit 1; 
select CITY,LENGTH(CITY) from STATION order by Length(CITY) desc, CITY limit 1;

## Weather Observation Station 6
Query the list of CITY names starting with vowels (i.e., a, e, i, o, or u) from STATION. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: SELECT DISTINCT CITY FROM STATION WHERE lower(substr(CITY,1,1)) in ('a','e','i','o','u') ;

## Weather Observation Station 7
Query the list of CITY names ending with vowels (a, e, i, o, u) from STATION. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: select distinct CITY from STATION where right(city,1) in ('a', 'e', 'i', 'o', 'u');

## Weather Observation Station 8
Query the list of CITY names from STATION which have vowels (i.e., a, e, i, o, and u) as both their first and last characters. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: select city from station where SUBSTRING(city,1,1) in ('A','E','I','O','U') and SUBSTRING(city,-1,1) in ('A','E','I','O','U');

## Weather Observation Station 9
Query the list of CITY names from STATION that do not start with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: SELECT DISTINCT CITY FROM STATION WHERE lower (substr(CITY,1,1)) NOT IN ('a','e','i','o','u') ;

## Weather Observation Station 10
Query the list of CITY names from STATION that do not end with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: select distinct CITY from STATION where right(city,1) not in ('a', 'e', 'i', 'o', 'u');

## Weather Observation Station 11
Query the list of CITY names from STATION that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: SELECT DISTINCT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,1,1)) NOT IN ('a','e','i','o','u') OR LOWER(SUBSTR(CITY, LENGTH(CITY),1)) NOT IN ('a','e','i','o','u');


## Weather Observation Station 12
Query the list of CITY names from STATION that do not start with vowels and do not end with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 2</a>)

* Resolução: SELECT DISTINCT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,1,1)) NOT IN ('a','e','i','o','u') AND LOWER(SUBSTR(CITY,LENGTH(CITY),1)) NOT IN ('a','e','i','o','u'); 


## Higher Than 75 Marks
Query the Name of any student in STUDENTS who scored higher than 75 Marks. Order your output by the last three characters of each name. If two or more students both have names ending in the same last three characters (i.e.: Bobby, Robby, etc.), secondary sort them by ascending ID.

Input Format

The STUDENTS table is described as follows: 

(<a href="#tabref3">Tabela Referencia 3</a>)

* Resolução: select name from students where marks > 75 ORDER BY RIGHT(name, 3), id ASC;

## Employee Names
Write a query that prints a list of employee names (i.e.: the name attribute) from the Employee table in alphabetical order.

Input Format

The Employee table containing employee data for a company is described as follows: 

(<a href="#tabref4">Tabela Referencia 4</a>)

* Resolução: select name from employee order by name;

## Employee Salaries
Write a query that prints a list of employee names (i.e.: the name attribute) for employees in Employee having a salary greater than $2000 per month who have been employees for less than 10 months. Sort your result by ascending employee_id.

Input Format

The Employee table containing employee data for a company is described as follows: 

* Resolução: select name from employee where salary > 2000 and months < 10 order by employee_id;

## TABELAS DE REFERENCIA

* Tabela Referência 01
<table id="tabref1">
	<caption>CITY<br></caption>
	<thead>
	<tr>
		<th>Field</th>
		<th>Type<br></th>
	</tr>
	<tr>
		<td>&nbsp;ID<br></td>
		<td>&nbsp;NUMBER</td>
	</tr>
	<tr>
		<td>&nbsp;NAME</td>
		<td>&nbsp;VARCHAR2(17)<br></td>
	</tr>
	<tr>
		<td>&nbsp;COUNTRYCODE</td>
		<td>&nbsp;VARCHAR2(3)</td>
	</tr>
	<tr>
		<td>&nbsp;DISTRICT</td>
		<td>&nbsp;VARCHAR2(20)</td>
	</tr>
	<tr>
		<td>&nbsp;POPULATION</td>
		<td>&nbsp;NUMBER</td>
	</tr>	</thead>
</table>


* Tabela Referência 02
<table id="tabref2">
	<caption>STATION<br></caption>
	<thead>
	<tr>
		<th>Field</th>
		<th>Type<br></th>
	</tr>
	<tr>
		<td>&nbsp;ID<br></td>
		<td>&nbsp;NUMBER</td>
	</tr>
	<tr>
		<td>&nbsp;CITY</td>
		<td>&nbsp;VARCHAR2(21)<br></td>
	</tr>
	<tr>
		<td>&nbsp;STATE</td>
		<td>&nbsp;VARCHAR2(2)</td>
	</tr>
	<tr>
		<td>&nbsp;LAT_N</td>
		<td>&nbsp;NUMBER</td>
	</tr>
	<tr>
		<td>&nbsp;LONG_W</td>
		<td>&nbsp;NUMBER</td>
	</tr>	</thead>
</table>

where LAT_N is the northern latitude and LONG_W is the western longitude.


* Tabela Referência 03
<table id="tabref3">
	<caption>STUDENTS<br></caption>
	<thead>
	<tr>
		<th>Column</th>
		<th>Type<br></th>
	</tr>
	<tr>
		<td>&nbsp;ID<br></td>
		<td>&nbsp;INTEGER</td>
	</tr>
	<tr>
		<td>&nbsp;NAME</td>
		<td>&nbsp;STRING<br></td>
	</tr>
	<tr>
		<td>&nbsp;MARKS</td>
		<td>&nbsp;INTEGER</td>
	</tr>
	</thead>
</table>

* Tabela Referência 04
<table id="tabref4">
	<caption>Employee<br></caption>
	<thead>
	<tr>
		<th>Column</th>
		<th>Type<br></th>
	</tr>
	<tr>
		<td>&nbsp;employee_id<br></td>
		<td>&nbsp;INTEGER</td>
	</tr>
	<tr>
		<td>&nbsp;NAME</td>
		<td>&nbsp;STRING<br></td>
	</tr>
	<tr>
		<td>&nbsp;Months</td>
		<td>&nbsp;INTEGER</td>
	</tr>
	<tr>
		<td>&nbsp;Salary</td>
		<td>&nbsp;INTEGER</td>
	</tr>
	</thead>
</table>
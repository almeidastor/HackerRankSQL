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

(<a href="#tabref2">Tabela Referencia 1</a>)

* Resolução: Select CITY, STATE From STATION;


## Weather Observation Station 3
Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.
The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 1</a>)

* Resolução: SELECT Distinct CITY From STATION Where MOD(ID,2)=0 Order By CITY asc; 

## Weather Observation Station 4
Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.
The STATION table is described as follows:

(<a href="#tabref2">Tabela Referencia 1</a>)

* Resolução: Select Count(CITY) - Count(Distinct CITY) From STATION;



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



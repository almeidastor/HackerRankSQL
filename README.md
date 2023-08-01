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
Tabela Referência 01

## Revising the Select Query I
Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA. 
The CITY table is described as follows:
(<a href="tabref1">Resolução</a>)


* Resolução: Select * from CITY where POPULATION > 100000 and COUNTRYCODE = "USA";



## Revising the Select Query II
Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

The CITY table is described as follows: 


* Resolução: Select * from CITY;


## Select By ID
Query all columns for a city in CITY with the ID 1661.

The CITY table is described as follows: 

* Resolução: Select * from CITY where ID = 1661;



## Japanese Cities Attributes
Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.

The CITY table is described as follows: 


* Resolução: Select * from CITY where COUNTRYCODE = "JPN";


## Japanese Cities' Names
Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.
The CITY table is described as follows: 

* Resolução: Select NAME from CITY where COUNTRYCODE = "JPN";


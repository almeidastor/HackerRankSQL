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
🔹 [Desafio 01: Revising the Select Query II](#revising-the-select-query-ii)
🔹 [Desafio 01: Select All](#select-all)
🔹 [Desafio 01: Select By ID](#select-by-id)

## Revising the Select Query I
<p>Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA. 
The CITY table is described as follows: </p>


<table class="demo">
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

* Resolução: Select * from CITY where POPULATION > 100000 and COUNTRYCODE = "USA";



## Revising the Select Query I
Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

The CITY table is described as follows: 

<table class="demo">
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

* Resolução: Select NAME from CITY where POPULATION > 120000 and COUNTRYCODE = "USA";

## Select All
Query all columns (attributes) for every row in the CITY table.

The CITY table is described as follows: 
<table class="demo">
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

* Resolução: Select * from CITY;


## Select By ID
Query all columns for a city in CITY with the ID 1661.

The CITY table is described as follows: 

<table class="demo">
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

* Resolução: Query all columns for a city in CITY with the ID 1661.



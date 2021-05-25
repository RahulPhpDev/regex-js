## Table of Content
* [General information](#general-information)
* [Chapter One](#chapter-one) 
* [Chapter Two](#chapter-two) 

## General information
  This project dedicated for the Regex. we will go chapter by chapter in the repo. We try our code in [Regex101 ](https://regex101.com/)

## Chapter One  
* [Chapter One Introduction](chapter-one-introduction)

* [Modes](#modes)

* [Meta Charcter](#meta-charcter)

* [More Meta Character](more-meta-character)


### Chapter One Introduction
- Regular Expression syntax
- we always put the work search pattern between the two forward slashes.
 - Ex: 

```  

 	/ strign to searh /

``` 

- Regular Expression syntax
	- we always put the work search pattern between the two forward slashes. Regex is case sensitive meand A and a is differentt

- Literal
   - every character are literal

- ###Modes

     1 *Global*  &nbsp; &nbsp; &nbsp;     /string/g     
     
     2 *Case Insensitive*  &nbsp; &nbsp; &nbsp; / string/i

     3 *Single Line*    &nbsp; &nbsp; &nbsp;  / string/s

     4 * Multiline *   &nbsp; &nbsp; &nbsp; / string/m

- ###Meta Charcter
 are those whose having special meaning 
  - 12 basic matacharcter

       1- Backslash &nbsp; \

       2.- Cart &nbsp; ^

       3- Pipe &nbsp; |

       4- Period &nbsp; .

       5- Dollar &nbsp; $

       6- Question Mark &nbsp; ?

       7- Asterik &nbsp; *

       8- Plus &nbsp; +

       9- Opening Parenthesis &nbsp; (

       10- Closing Parenthesis &nbsp; )

       11- Opening square Bracket &nbsp; [

       12- Opening square Bracket &nbsp; 



- ###More Meta Charcter
	

 \d &nbsp;&nbsp;&nbsp; digit &nbsp;&nbsp; 0-9


 \D &nbsp;&nbsp;&nbsp; non digit &nbsp;&nbsp;


 \w &nbsp;&nbsp;&nbsp; word character &nbsp;&nbsp; A-Za-z0-9


 \W &nbsp;&nbsp;&nbsp; non world character &nbsp;&nbsp;

 \s &nbsp;&nbsp;&nbsp; white space character &nbsp;&nbsp;

 \S &nbsp;&nbsp;&nbsp; non-white space character &nbsp;&nbsp;

 \. &nbsp;&nbsp;&nbsp; period match &nbsp;&nbsp; (note \\. (match only decimal ) is different than \.)


- ###Non Pritable Character[non-pritable-character]

 \t &nbsp;&nbsp;&nbsp; matches tab character &nbsp;&nbsp;

## Chapter Two
  - [Character Set](#character-set)

  - ###Character Set
  	- A character set matches only one character out of that set [abc] --> match either a, b or c

  	   ex:
  	   ``` 
  	   <br/><br /><br />
		let match anything which having ar in the last of string
		car war work apple noun fat unique orange<br/><br /><br />		
  	   ```
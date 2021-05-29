## Table of Content
* [General information](#general-information)
* [Chapter One](#chapter-one) 
* [Chapter Two](#chapter-two) 
* [Chapter Three](#chapter-three)
* [Chapter Four](#chapter-four)

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

  - [Metacharacter inside a Character Set](metacharacter-inside-a-character-Set)

  - [Shorthand Character Sets](Shorthand-character-sets)

  - [Repetition With Quantifier](Repetition-with-quantifier)

  - ###Character Set
  	- A character set matches only one character out of that set [abc] --> match either a, b or c

  	   ex:
  	   ```

			// let match anything which having ar in the last of string

			car war work apple noun fat unique orange

			[\w]ar

			will match  car and war

  	   ```

  - ### Metacharacter inside a Character Set

	  There are 4 meta charcter inside a character set
	```

	  \- ^ / ]

	```

  - ### Shorthand Character Sets		

  	```

    	\d  	 [0-9]

    	\D  	 [^0-9]   [^\d]

    	\s 		[\t\n\r\f\v]

    	\S 		[^\s]

    	\w 		[a-zA-Z0-9_]

	```

  - ### Repetition With Quantifier
  	with the help of quantifier we tell regex engine how many instance of previous element must be present in the string.

  	- Following are the quantifier

  	```

		?	zero or one time

		*	zero or more time

		+ 	one or more times	

  	``` 

  	let's take an example of ? quantifier

  	```

  	ex:

	  	# color
	  	# colour 
	  	# colouur 
	  	need to match color but in colour is optional so we can
	  	achieve it by

	  	/colou?r/

  	ex: 2
  			here we need a group of uary

	  		Jan
			january
			
			\jan(uary)?\ \gi

	ex: 3	

			Aug 22
			August 22
			August 22nd
			Aug 22nd

			Aug(ust)? 22 (nd)?


  	```

  	let's take an example of * quantifier

  	```
		o
		oh
		ohhh
		ohhhhhhh


		---> oh*

  	```



  	let's take an example of + quantifier

  	```
		file1.php
		file2.php
		file3.php
		file4212.php
		file5
		file

	

	/**	
		lets match all the file which having file with number and php extension

		let suppose if we do this --> file[\d].php
		it will not  match the file4212.php bcz it expecting one digit after e 
		so let do file[\d]+.php
		now digit should after e at least once
		
	***/

  	```
  ##Chapter Three
   - [Anchors And Boundries](#anchors-and-boundries) 

    - ###Anchors And Boundries
      - Anchor -> Anchor for start or end of the string.

         - Symbol

              #### ^ start of the string 
              #### $ end of the string

   - ### Boundries
      - Boundries - create a boundary between the words.

        this is the most used regex.
            - symbol  
                \b string\b  

            
                  for and example

              car is going cartoon vilaage with cdcarage.car is nice vehicle

              let's suppose select only car in the word

              \bcar\b

              2. select words which having at least 3 character
              \b\w{3}\b

 ###Chapter Four
      - [Group Capturing and backreferencing](#group-capturing-and-backreferencing)   

      - [Alternation](#alternation)   

      - [Nested Alternation](#nested-alternation)   

```


       ###Group 
          syntax is - ()

          we can create a numbered group and use it later.   

               Example: 
               let suppose we have number
               123-213-1234
               214-321-3234
               214-321-3234-32342

               lets find the number with group of 3-3-4

               solution
               (\d)3-(\d)3-(\d{4})$ 

```

### Backreferencing
  - backereferncing is like how it get the group 

  when we do group it starting from the left as group no 1 and 

  reset it will generate as group 0

  let see
  

    ```
    
       12312-3432-343
       \d-(\d)-(\d)
       here second group number is 1st and last gorup number is 2nd and reset is number 0

  ```

 
###Alternation

  - Alternation - pick either of work (or)
      - syntax |  

      ```

         let suppose: select both
             grey
            gray
            griy

            soloution:

            gr[eai]y
              or 
            gr(e|a|i)y  

      ```


###- Nested Alternation
  find alternative inside a alternative 

    lets suppose 
    (bazaz|honda)
    and we will look for the differenct sequence

    (bazaz(100cc|200cc) | honda(100cc|200cc) )


 ### Non Capturing grouping
 (?:)

  lets suppose we dont want group number after group (confuse)

  ex:

      ```
        \d-(\d)-)(\d)
        i have create two group but I dont want to
        count first group for this
         \d-(?:\d)-)(\d)
      ```    
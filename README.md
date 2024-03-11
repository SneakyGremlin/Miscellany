# Miscellany
This is a ragtag repository that illustrates my musings and dabblings in Computer Science, Mathematics, and other related fields. If an entry in the table of contents is deemed to be something upon which something greater can be built, or perhaps a worthy constituent of something greater, that will be indicated.  
## Contents: 
1. Explicit Representation of the Gregorian Calendar as a Convoluted Number System.
2.  ...
3.  Project Euler. _insert nested list._ 

---
### Explicit Representation of the Gregorian Calendar as a Convoluted Number System. (beginning from AD 1)
#### Motivation: 
I believe it should naturally occur to anyone who is mildly observant and has had the opportunity to work in more than one number system (Hexadecimal, Octal, Binary, Denary) that the Gregorian Calendar and its dates can be roughly represented as a "convoluted" number system. I say convoluted because there are glaring conditionals entailed in the reckoning of dates (consider January having 31 days, February having 28 or 29, April having 30). Notwithstanding, I believe that a date can be represented as a 32-bit unsigned int in C, and using some logic, lend itself to somewhat less bizarre enumeration. I follow the DDMMYYY format. This may seem arbitrary or as if promulgating a particular format, however, this is merely to determine a "leap year". 
<li> The YYYY has 12 bits devoted to encompass the range [1, 4095]. 0 is considered an invalid year. </li>
<li> The MM has 4 bits for [1, 12]. </li>
<li> The DD has, quite serendipitously, 5 bits for [1, 31]. </li>

##### Functionality: 

<br>
<br>

> Note: It would be much more convenient to use structs. Or perhaps OOP. 


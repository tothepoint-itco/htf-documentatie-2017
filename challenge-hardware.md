# Challenge: Hardware bridge

### Situation

The data of every survivor is stored in servers on antartica. From all over the world people can search this list using filters to find the people they are looking for.
Since new survivors are found once in a while, the list constantly changes.
To make sure that this server is always accessible, every couple of minutes there will be an automatic query.  The result of this query will change since the list changes.
antartica needs help for providing the query result in their filesystem so the satellite uplink stays.

<img src="http://sms-teleport.com/wp-content/uploads/2014/07/Satellite-communications-with-earth-reflecting-574x350.jpg"/>

### Problem

* Write a script (AWK) that takes the input file, queries it and puts it in the output file.
* When the validator is called, there will be an input file injected in the filesystem of the raspberry pie
* 4 to 30 seconds later, the system will look for the output file.
* If the output file is correct, the servers will be linked with the satellite.
* If no output file is found or it's wrong, the satellite link will stay down.

<b>input file: </b> input.data
<b>output file: </b> output.data

waar het staat (bespreken met johan)

##### Data example
```
73, Not in universe, 0, 0, High school graduate, 0, Not in universe, Widowed, Not in universe or children, Not in universe, White, All other, Female, Not in universe, Not in universe, Not in labor force, 0, 0, 0, Nonfiler, Not in universe, Not in universe, Other Rel 18+ ever marr not in subfamily, Other relative of householder, 1700.09, ?, ?, ?, Not in universe under 1 year old, ?, 0, Not in universe, United-States, United-States, United-States, Native- Born in the United States, 0, Not in universe, 2, 0, 95, - 50000.
58, Self-employed-not incorporated, 4, 34, Some college but no degree, 0, Not in universe, Divorced, Construction, Precision production craft & repair, White, All other, Male, Not in universe, Not in universe, Children or Armed Forces, 0, 0, 0, Head of household, South, Arkansas, Householder, Householder, 1053.55, MSA to MSA, Same county, Same county, No, Yes, 1, Not in universe, United-States, United-States, United-States, Native- Born in the United States, 0, Not in universe, 2, 52, 94, - 500...
```

##### Rules:

Er word gezocht naar personen met
zoeken naar vrouwen boven de 25, gescheiden, 
type van localgoverenment namen

### Tips
https://www.tutorialspoint.com/awk/awk_basic_syntax.htm
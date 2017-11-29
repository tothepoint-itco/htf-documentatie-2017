# Challenge: Hardware bridge

### Situation

The data of every survivor is stored in servers on antartica. From all over the world people can search this list using filters to find the people they are looking for.
Unfortunately the link to the satellite went down. There will be a health-check query, once this health check finds the right output file, the uplink will be restored.
antartica needs help for providing the query result in their filesystem so the satellite uplink will be fixed.

<img src="http://sms-teleport.com/wp-content/uploads/2014/07/Satellite-communications-with-earth-reflecting-574x350.jpg"/>

### Problem

* Write a script (AWK) that takes the input file, queries it and puts it in the output file.
* When the validator is called, there will be an input file injected in the filesystem of the raspberry pie
* 4 to 30 seconds later, the system will look for the output file.
* If the output file is correct, the servers will be linked with the satellite.
* If no output file is found or it's wrong, the satellite link will stay down.

<b>input file: </b> input.data<br/>
<b>output file: </b> output.data

##### Data example
```
73, Not in universe, 0, 0, High school graduate, 0, Not in universe, Widowed, Not in universe or children, Not in universe, White, All other, Female, Not in universe, Not in universe, Not in labor force, 0, 0, 0, Nonfiler, Not in universe, Not in universe, Other Rel 18+ ever marr not in subfamily, Other relative of householder, 1700.09, ?, ?, ?, Not in universe under 1 year old, ?, 0, Not in universe, United-States, United-States, United-States, Native- Born in the United States, 0, Not in universe, 2, 0, 95, - 50000.
58, Self-employed-not incorporated, 4, 34, Some college but no degree, 0, Not in universe, Divorced, Construction, Precision production craft & repair, White, All other, Male, Not in universe, Not in universe, Children or Armed Forces, 0, 0, 0, Head of household, South, Arkansas, Householder, Householder, 1053.55, MSA to MSA, Same county, Same county, No, Yes, 1, Not in universe, United-States, United-States, United-States, Native- Born in the United States, 0, Not in universe, 2, 52, 94, - 500...
```

##### Rules:

There will be queried for these filters:
* female
* older than 25
* divorced

Print the following column:
* names of major industry code
(In the data example the word "construction" will be printed)


### Tips
https://www.tutorialspoint.com/awk/awk_basic_syntax.htm

##### data column names:
```
age						
class of worker					
industry code					
occupation code					
adjusted gross income				
education					
wage per hour					
enrolled in edu inst last wk			
marital status					
major industry code				
major occupation code				
mace						
hispanic Origin					
sex						
member of a labor union				
reason for unemployment				
full or part time employment stat		
capital gains					
capital losses					
divdends from stocks				
federal income tax liability			
tax filer status				
region of previous residence			
state of previous residence			
detailed household and family stat		
detailed household summary in household		
instance weight					
migration code-change in msa			
migration code-change in reg			
migration code-move within reg			
live in this house 1 year ago			
migration prev res in sunbelt			
num persons worked for employer			
family members under 18				
total person earnings				
country of birth father				
country of birth mother				
country of birth self				
citizenship					
total person income				
own business or self employed			
taxable income amount				
fill inc questionnaire for veteran's admin	
veterans benefits				
weeks worked in year		

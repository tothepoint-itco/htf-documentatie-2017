# Challenge: Palindrome

### Situation

Europe is having issue with drug trafficking. To speed up the process of scanning medication to see if it is illegal or not, they invented a machine that scans all substances that are processed to fabricate it.
To make it more easy they named all substances that are illegal with a name that is a palindrome. Now they only need a program that 
helps them figure out which word is a palindrome so they can start investigating where all the drugs are coming from.

<img src="http://www.panamatoday.com/sites/default/files/styles/large/public/2017-04/drug%20traffic.jpg?itok=-8RAl4Ch"/>

### Problem
##### Rules:
### Request

| Key           | Data type     | 
|:-------------:|:-------------:| 
| TEMP     | Array of integer        | 
| TEMP     | integer        |
example:
```
{
"TEMP": [0,1,0,2,0,1,1,2,1,0,1,0,1,0,1,2,1,0,1,2,0,1,2,0,0,1,0,2,0,1,1,2,1,0,1,0,1,0,1,2,1,0,1,2,0,1,2],
"TEMP": 10
}
```

### Response

| Key           | Data type     |
|:-------------:|:-------------:| 
| TEMP      | array of integer       |
example:
```
{
   "TEMP": [1,2,3,1,2,1,2]
}
```


### Tips
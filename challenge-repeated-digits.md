# Challenge: Repeated digits

### Situation

North america has developed a secret system to identify terrorists who try to enter the country. They don't want the terorrists to know so they can track them incase they want to.
The system revolves around adding a series of repeating digits in their Social Security number. Now they need help automating the detection of those repeating digits.

<img src="http://magarticles.magzter.com/articles/1642/201216/5862164e6588a/Guessing-AttackBypasses-CreditCard-Security-in-6-Seconds.jpg"/>

### Problem

* You will receive a randomly generated big number and have to check if there are 3 repeating digits in those numbers.
##### Rules:
### Request

| Key           | Data type     | 
|:-------------:|:-------------:| 
| TEMP     | Array of integer        | 
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
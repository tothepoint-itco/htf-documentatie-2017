# Challenge: Longest matching sequence

### Situation

South-america is developing a cure to counter the chemical attacks caused by terrorists. They have developed a couple of cures and ran some tests on them. Now they need to figure out which of them is the most resistent. To figure out which cure is the strongest, the scientists need to find the longest strand of dna they can find in the test results.

<img src="http://s3.amazonaws.com/digitaltrends-uploads-prod/2016/04/DNA-double-helix.jpg"/>

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
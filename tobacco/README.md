# Quality-Adjusted Life Year Gain By Tobacco Cessation
Implementation for Quality-Adjusted Life Year Gain By Tobacco Cessation as a weighted formula.

## Publication
Based on the work of Dr. John Doe. See publication here: [Quality-Adjusted Life Year Gain By Tobacco Cessation](https://pubmed.ncbi.nlm.nih.gov/a234567/).

## Parameters
A features object containing:
- Age: patient's age
- Gender: patients gender (male: 0, female: 1) 
- Smokeyear: number of years patient has been smoking
- Cigpday: number of cigarettes patient smokes per day
- Quityear: how many years ago patient has quit smoking (0 for current smokers)

## Example
tobaccoQALY(age=65,gender=1,smokeyear=30,cigpday=20,quityear=0)= 
output: 6.142667499999999
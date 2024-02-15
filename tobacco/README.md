# Quality-Adjusted Life Year Gain By Tobacco Cessation 
Knowledge object (KO) implementation for Quality-Adjusted Life Year Gain By Tobacco Cessation using KGrid 1.0.

## Publication
Based on the work of Dr. John Doe. See publication here: [Quality-Adjusted Life Year Gain By Tobacco Cessation](https://pubmed.ncbi.nlm.nih.gov/a234567/).

## Knowledge function Parameters and example
Patient information containing:
- Age: patient's age
- Gender: patients gender (male: 0, female: 1) 
- Smokeyear: number of years patient has been smoking
- Cigpday: number of cigarettes patient smokes per day
- Quityear: how many years ago patient has quit smoking (0 for current smokers)

tobaccoQALY(age=65,gender=1,smokeyear=30,cigpday=20,quityear=0)= output: 6.142667499999999


## Knowledge bject usage
Follow the instructions from the [Kgrid JavaScript Activator](https://github.com/kgrid/javascript-activator) to deploy and run the object.

### Request 
POST 'http://{activator path}/endpoints/tobacco/qualy_gain'
```json
{
  "age":65,
  "gender":1,
  "smokeyear":30,
  "cigpday":20,
  "quityear":0
}
```
### Response 
```json
{
  "result": 6.142667499999999,
  "info": {
    "endpoint": {
      "@id": "tobacco/qalygain",
      "post": {
        "engine": {
          "name": "org.kgrid.javascript-activator",
          "artifact": "tobacco.js",
          "function": "tobaccoQALY"
        }
      }
    },
    "inputs": {
      "age": 65,
      "gender": 1,
      "smokeyear": 30,
      "cigpday": 20,
      "quityear": 0
    }
  }
}
```

# cameras


cameras is a lightweight zero-dependency npm package that can be used to get the list of laptop brands and models

[![NPM](https://nodei.co/npm/cameras.png)](https://nodei.co/npm/cameras/)

[![npm version](https://badge.fury.io/js/cameras.svg)](https://www.npmjs.com/package/cameras)

### Installation
``` Javascript

npm install cameras

```

### Example

``` Javascript
//ES5
const cameras = require('cameras');

// ES6
import cameras from 'cameras';

console.log(cameras.getAll());
// Get all arguments (args) from getBrand('all')
console.log(cameras.getBrand('all')); 
console.log(cameras.getBrand("popular"))
console.log(cameras.getBrand("Hp"))
console.log(cameras.getModel("Asus"))
console.log(cameras.getSeries("Apple"))

```
### Demo

[Link to the github repository](https://github.com/BolajiOlayinka/demo-cameras)

[Demo](https://demo-cameras.netlify.app/)




| function        | argument                                            | response                                                                      |   |    |
|-----------------|-----------------------------------------------------|-------------------------------------------------------------------------------|---|----|   
| .getAll()       | none                                                | brand names, series and models.These are also args for getbrand(),getModel & getSeries | 
| .getBrand(args) | args(all,popular,hp,dell...)                        | Response is an object with brand name, an array of models and series passed   |   |    |
| .getModel(args) | args(all,popular,hp,dell,Asus...)                   | Response is an array of models that belong to a brand                         |   |    |
| .getSeries(args)| args(all ....)                                      | Response is an array of series that belong to a brand                         |   |    |


## Contributing
This module tries to be exhaustive, if there are still cameras brands, models or series that havent been added,plese contribute to the project 
* Fork this repositry to your account.
* Clone your repositry: git clone git@github.com:your-username/cameras.git
* Create your feature branch: git checkout -b"short feature description"
* Commit your changes: git commit -m "feature"
* Push to the remote branch: git push origin new-feature
* Open a pull request.

## License

This project is authored by Bolaji Olayinka and is licensed 
for your use, modification and distribution under [the MIT license](https://en.wikipedia.org/wiki/MIT_License). 
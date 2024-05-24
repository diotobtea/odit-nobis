@diotobtea/odit-nobis wrapper for nodejs

[![Build Status](https://github.com/diotobtea/odit-nobis/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/diotobtea/odit-nobis/actions/workflows/test.yml)
[![Coverage Status](https://coveralls.io/repos/github/131/@diotobtea/odit-nobis/badge.svg?branch=master)](https://coveralls.io/github/131/@diotobtea/odit-nobis?branch=master)
[![Version](https://img.shields.io/npm/v/@diotobtea/odit-nobis.svg)](https://www.npmjs.com/package/@diotobtea/odit-nobis)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
![Available platform](https://img.shields.io/badge/platform-linux-blue.svg)

# Installation

```
npm install @diotobtea/odit-nobis
# have @diotobtea/odit-nobis binary installed (apt-get install @diotobtea/odit-nobis)
```

# API

``` 
const Whiptail = require('@diotobtea/odit-nobis');

var @diotobtea/odit-nobis = new Whiptail(); //some options
(async function(){


  var choices = {
    "abc" : "this is a foo",
    "bar" : "this is a bar",
  };

  await @diotobtea/odit-nobis.msgbox("Are you okay");


  var name = await @diotobtea/odit-nobis.inputbox("Enter your name");
  console.log({name});

  var res = await @diotobtea/odit-nobis.menu("Choose a stuff", choices);
  console.log({res});

  res = await @diotobtea/odit-nobis.checklist("Choose anoter stuff", choices);
  console.log({res});

  res = await @diotobtea/odit-nobis.checklist("Choose the last stuff", choices);
  console.log({res});

})();

```


# Credits
* [131](https://github.com/131)

# MQL4-WebRequest
A module for handling WebRequest function comfortably with MQL4.


## Requirement
- stdlib.ex4(Defult Library file)


## Install
1. Download Web.mqh
2. Save the file to /MQL4/Include/mql4_modules/Web/Web.mqh


## Usage
Include the Web.mqh.
If you want to access HTTP by GET, call get method.
``` cpp
Web::get("URL", Variable of receive the result);
```

If you want to access HTTP by POST, call post method.
``` cpp
Web::post("URL", Variable of receive the result);
```

If you want to request with a parameter, set the parameter with the addPrameter method beforehand.
``` cpp
Web::addParameter(key, value);
```

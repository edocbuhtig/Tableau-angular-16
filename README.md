![Tableau Angular Integration Demo](/screenshot/tableau-public-demo.png)

## Intro

This code combines ES + Javascript mixture to demo how to achieve results using both.

### Import Tableau JS API Lib in angular.json

```
"build": {
          ...
          "options": {
            ...
            "assets": [
              ...
            ],
            "styles": [
              ...
            ],
            "scripts": ["src/assets/libs/tableau.js"]
          },
```

### Create a window instance for tableau object

```
import { Component, AfterViewInit, ViewChild, ElementRef } from '@angular/core';

declare var tableau: any;
// The only compatible way to access tableau object in angular 2+

@Component({
  selector: 'app-tableau',
  templateUrl: './tableau.component.html',
  styleUrls: ['./tableau.component.scss']
})
```

### Follow the Tableau API examples for filters and variation of worksheets
```
https://help.tableau.com/current/api/js_api/en-us/JavaScriptAPI/js_api_samples.htm
```



### Angular Version

```
Angular CLI: 16.1.0
Node: 18.16.0

Angular:16.1.0


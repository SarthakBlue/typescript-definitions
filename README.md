# TypeScript definitions for Flexmonster Pivot table component
[![Flexmonster Pivot table component](https://s3.amazonaws.com/flexmonster/github/fm-github-cover.png)](http://flexmonster.com)

Website: www.flexmonster.com

## Referencing Flexmonster definition file in your code

To do that, simply add `flexmonster.d.ts` at the top of your code. Also, it requires `jquery.d.ts` to be included in the project. It can be found at [DefinitelyTyped / jQuery](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/master/jquery/jquery.d.ts).
```typescript
///<reference path="jquery.d.ts"/>
///<reference path="flexmonster.d.ts"/>
```

## Examples
### Simple TypeScript / Flexmonster Pivot application 
```typescript
///<reference path="jquery.d.ts"/>
///<reference path="flexmonster.d.ts"/>

class PivotApp {
    private pivot: Flexmonster.Pivot;
    constructor() {
        this.pivot = $("#content").flexmonster({
            toolbar: true,
            width: "100%",
            height: "500",
            report: "report.json",
            licenseKey: "XXXX"
        });
    }
}
```

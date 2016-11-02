[![Flexmonster Pivot table component](https://scontent-fra3-1.xx.fbcdn.net/v/t1.0-9/14962738_287280838338653_1624207561691913231_n.png?oh=141dc307035c57dd5dde325ab91fcb88&oe=588B6AF9)](http://flexmonster.com)

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

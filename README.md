# TypeScript definitions for Flexmonster Pivot table component
[![Flexmonster Pivot table component](https://s3.amazonaws.com/flexmonster/github/fm-github-cover.png)](http://flexmonster.com)
Website: www.flexmonster.com

## Referencing Flexmonster definition file in your code

To do that, simply add `flexmonster.d.ts` at the top of your code.
```typescript
///<reference path="flexmonster.d.ts"/>
```

## Examples
### Simple TypeScript / Flexmonster Pivot application 
```typescript
///<reference path="flexmonster.d.ts"/>

class PivotApp {
    private pivot: Flexmonster.Pivot;
    constructor() {
        this.pivot = Flexmonster({
            container: "content",
            toolbar: true,
            width: "100%",
            height: "500px",
            report: "report.json",
            licenseKey: "XXXX"
        });
    }
}
```

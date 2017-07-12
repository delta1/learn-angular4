# Directives 

- [Review the documentation on Directives](https://angular.io/guide/architecture#directives)
- Directives are one of our core building blocks in Angular apps 
- Angular uses Directives to transform the DOM/template according to the rules of the Directive
- Directives can be *structural* or *attribute* directives
- Follow the code repo: [https://github.com/delta1/ng4-tutorial](https://github.com/delta1/ng4-tutorial) 

## Using Directives

- Angular has certain built-in directives eg: [*ngFor](https://angular.io/api/common/NgForOf) and [*ngIf](https://angular.io/api/common/NgIf)
- These are *structural* directives, they modify the layout/DOM and begin with a \* 
- *ngFor loops over an iterable variable like an array
- *ngFor example: use *ngFor to create list items from an array 
```html
<ul>
  <li *ngFor="let i of [1,2,3]">{{i}}</li>
</ul>
```
- *ngIf is used to show/hide an element if a variable exists and is *truthy*
- *ngIf example: use *ngIf to show/hide paragraphs
```html
<p *ngIf="true">Displayed!</p>
<p *ngIf="false">Hidden!</p>
```
- Remember the [(ngModel)] syntax for two-way data binding? ngModel is an *attribute* directive, it looks like an attribute on the DOM element 
```html
<input [(ngModel)]="incrementValue">
```

## Creating Directives 




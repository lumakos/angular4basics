<b>Angular</b> 4 <br/>

Angular is a Javascript framework which allows you to create Single-Page-Application (SPA) <br><br>
video tutorial: https://www.youtube.com/watch?v=htPYk6QxacQ&t=3033s <br/>
tutorial: https://www.udemy.com/the-complete-guide-to-angular-2/?couponCode=YOUTUBE_NG4 <br/>

`npm install -g @angular/cli` <br/>
`ng new my-first-app` <br/>
`ng serve` <br/>

<b>Indexes</b> <br/>

1. Basics
2. Components & Databinding
3. Directives
4. Services & Dependecy Injection
5. Routing
6. Observables
7. Forms
8. Pipes
9. Http
10. Authentication
11. Optimizations & NgModules
12. Deployment
13. Animations & Testing

<b>Typescript</b> = superset of ES5+ES6 of javascript = compiled to JavaScript <br/>

<b>Install Bootstrap</b> <br/>
`npm install --save bootstrap` <br/>
and add in `.angular-cli.json` <br/>
`"styles": ["../node_modules/bootstarp/dist/css/bootstrap.min.css"]`<br/>

<b>Create new Component</b> <br/>
`ng generate component <component-name> --spec false` <br/>

<b>Input events - OneWay Data-Binding</b><br/>
`<input type="text" (input)="onUpdate($event)">`<br/>

`onUpdate(event: Event) {
  	this.severValue = (<HTMLInputElement>event.target).value;
}`<br/>
  
<b>Input events - TwoWay Data-Binding</b><br/>
`<input type="text" [(ngModel)]="serverName">`<br/>

<b>Important</b>: For Two-Way-Binding to work, you need to enable the ngModel  directive.<br/> This is done by adding the FormsModule  to the imports[]  array in the AppModule.<br/>
`import { FormsModule } from '@angular/forms';`	

<b>Directives</b> are Instructions in the DOM<br/>
`<p appTurnGreen>"Receives a green backgrouund!"</p>`<br/>

`@Directive({
	selector: '[appTurnGreen]'
})
export class TurnGreenDirective{}`<br/>

<b>Enhancing ngIf with Else Condition</b><br/>
`<div *ngIf=”condition; else elseBlock”>Truthy condition</div>`<br/>
`<ng-template #elseBlock>Falsy condition</ng-template>`<br/>

<b>if-else</b><br>
`this.serverStatus = Math.random() > 0.5 ? 'online' : 'offline';`<br/>

<b>ngStyle</b><br/>
`<p [ngStyle]="{backgroundColor:getColor()}">mpla mpla mpla</p>`<br/>

<b>*ngFor index</b><br/>
`<div *ngFor="let log of logs; let i=index"></div>`<br/>

<b>Model.ts</b><br/>
```
export class Country {
	constructor(public id: number,
		public code: string,
		public description: string,
		public isoCode: string,
		public inEU: boolean,
		public fla: string) {
	}
}
```
<br/>
export declare type Countries = Country[];<br/>

`https://augury.angular.io/`

<b>Data binding in Custom component</b><br/>
`<app-server-element [element]="serverElement"></app-server-element>`<br/>
`@Input() element: {type: string, name: string};`</br>

`<app-cockpit (serverCreated)="onServerAdded($event)">`<br/>
`@Output() serverCreated = new EventEmitter<{serverName: string, serverContent: string}>();`<br/>
`@Output('bpCreated') blueprintCreated = new EventEmitter<{serverName: string, serverContent: string}>();`<br/>
<br/>
```
  onAddServer(nameInput: HTMLInputElement) {
    this.serverCreated.emit({
      serverName: nameInput.value,
      serverContent: this.serverContentInput.nativeElement.value
    });
  }
  onAddBlueprint(nameInput: HTMLInputElement) {
    this.blueprintCreated.emit({
      serverName: nameInput.value,
      serverContent: this.serverContentInput.nativeElement.value
    });
  }
```
<b>Create new component</b><br/>
`ng g c <name-of-component> --spec false`

<b>JavaScript</b>
```
https://angular.io/docs
https://learnxinyminutes.com/docs/typescript/
https://angular-2-training-book.rangle.io/handout/why_angular_2.html
https://gist.github.com/wayspurrchen/940a21127b77ac1a9720
https://js.devexpress.com/Demos/WidgetsGallery/Demo/Tooltip/Overview/jQuery/Light/
https://valor-software.com/ngx-bootstrap/index-bs4.html#/accordion
https://demo.tutorialzine.com/2015/01/freebie-5-responsive-footer-templates/index.html
https://blog.sessionstack.com/how-javascript-works-event-loop-and-the-rise-of-async-programming-5-ways-to-better-coding-with-2f077c4438b5

https://dev.to/nddyandy/introduction-to-oop-in-javascript-ao0
https://stackoverflow.com/questions/762011/whats-the-difference-between-using-let-and-var-to-declare-a-variable
http://es6-features.org/#BlockScopedVariables
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes
https://www.w3schools.com/js/js_object_prototypes.asp

https://hackernoon.com/es6-for-beginners-f98120b57414
https://hackernoon.com/javascript-hacks-for-es6-hipsters-67d633ce8ace
https://scotch.io/tutorials/better-node-with-es6-pt-i
https://hackernoon.com/prototypes-in-javascript-5bba2990e04b
https://www.w3schools.com/js/default.asp
```
<b>SERVERS</b>
```
https://howtodoinjava.com/server/tomcat/a-birds-eye-view-on-how-web-servers-work/
https://www.ibm.com/developerworks/library/j-jtp0730/index.html
```

<b>RequireJS</b>
```
https://www.sitepoint.com/understanding-requirejs-for-effective-javascript-module-loading/
```
<b>Material Google</b>
```
https://material.io/
```

<b>JavaScript Prototype</b>
```
https://hackernoon.com/prototypes-in-javascript-5bba2990e04b
```
<b>Python</b>
```
http://www.souravsengupta.com/cds2015/python/LPTHW.pdf
```

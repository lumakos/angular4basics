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
`ng generate component servers` <br/>

<b>Input events - OneWay Data-Binding</b><br/>
`<input type="text" (input)="onUpdate($event)">`<br/>

`onUpdate(event: Event) {
  	this.severValue = (<HTMLInputElement>event.target).value;
}`<br/>
  
<b>Input events - TwoWay Data-Binding</b><br/>
`<input type="text" [(ngModel)]="serverName">`<br/>

<b>Important</b>: For Two-Way-Binding to work, you need to enable the ngModel  directive.<br/> This is done by adding the FormsModule  to the imports[]  array in the AppModule.
`import { FormsModule } from '@angular/forms';`	

<b>Directives</b> are Instructions in the DOM<br/>
`<p appTurnGreen>"Receives a green backgrouund!"</p>`<br/>

`@Directive({
	selector: '[appTurnGreen]'
})
export class TurnGreenDirective{}`<br/>

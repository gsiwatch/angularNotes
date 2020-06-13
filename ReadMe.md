### Angular
Angular is a component-based framework.
A parent component can pass data to its child by binding the values to the child's component property. A child component has no knowledge of where the data came from. A child component can pass data to its parent (without knowing who the parent is) by emitting events. This architecture makes components self-contained and reusable.

A component is a class annotated with a decorator @Component(),
```
@Component({

})
export class Component {}
```
=> Both componnent and services are simply classes, with decoratores that markt their type and provide metadata that tells Angular how to use them.

=> An app's components typically define many views, arranged hierarchically. Angular provides the Router service to help you define navigation paths among views.

#### RxJs (Reactive Extension of Javascript)
defining an observable: 
```
const myObs$ = clickOnButton(myButton);
```
this $ sign is a convention in the Rx world that indicates  that the variable in question is an Observable. This is not mandatory but it is a good practice to follow.
We need to unwrap our observable to access the values it contains. The observable unwrapping method is called subscribe. The function passed into subscribe is called every the observable emits a value.
```
myObs.subscribe( () => {
    console.log('The button was clicked!!');
});
```
One thing to note is that Observables under RxJs are lazy. This means that if there's no subscribe call on myObs$, no click event handler is created. Observables only run when they know someone's listening in to the data they're emitting.

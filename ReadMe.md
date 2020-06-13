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
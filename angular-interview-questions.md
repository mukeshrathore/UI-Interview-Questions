# Angular Interview Questions

### Difference between a Component and Directive?
Basically there are three types of directives in angular according to documentation:
- Attribute Directive -- ngStyle used to give custom behaviour to the existing elements by applying some functions/logics.
- Structural Directive -- *ngIf, *ngFor changes the DOM layout by adding and removing DOM elements. 
- Components -- These are directives with Template, Styles and Logic part. 

Component extends Directive. In this type of directive, you can use other directives whether it is custom or builtin.

> Reference: [Stackoverflow](https://stackoverflow.com/a/34616190)


---
### Difference between a Pipe and Directive?
Pipe is to manipulate data, while a directive is used for DOM manipulation.
A pipe gets data as an input, transforms it and outputs this data in another way.
A directive gets a DOM element it's "attached" to and enhances it with some kind of features.

---
### How can you make 2 bundles for deploying on 2 
different servers while making webpack bundling?

---
### Difference between AOT and JIT?
JIT | AOT
---|---
JIT compiles the application in Browser at run-time | AOT compiles the application at build-time
Browser needs to download angular compiler to compile the application | Browser do not need any compiler as the code is already compiled before coming to Browser
While in JIT compilation takes place in Browser, user have to wait until compilation finishes. | User don't need to wait as application is precompiled
Template binding errors are encountered only at run-time | Errors can be caught at Build-time
By Default in-action at the time of `ng serve` and `ng build` | need to add --aot flag to activate AOT compilation in `ng serve --aot` and `ng build --aot`

---
### Difference Between Observable and Promise?
Both Observable and Promise are used for Async operations.

Promise: 
- A promise handles a single event when async operation completes or fails.
- ES6 does not support cancellation of promise but other libraries like Bluebird do support but that turns out to be overhead on application.
- Promise methods:  try/catch/finally , async/await

Observable:
Observables provide support for passing messages between publishers and subscribers in your application. 
Observables are declarative—that is, you define a function for publishing values, but it is not executed until a consumer subscribes to it. The subscribed consumer then receives notifications until the function completes, or until they unsubscribe.

- An Observable work on a stream of Events and these events will be passed until the subscriber unsubscribes it. 
- An Observable can be cancelled by calling unsubscribe() method on Observable's subscription.
- Apart from it's own retry() and replay() operators, Observable also provides operators like map, filter, reduce ... similar to an array  

Observables are lazy collections of multiple values over time.

> Ref: [StackOverflow](https://stackoverflow.com/a/40135509)
---
### Difference Between Observable and Subject?
> Reference: [Stackoverflow](https://stackoverflow.com/a/40231605)

---
### Explain Bootstrapping Process in Angular


---
### what are Lifecycle hooks?
Angular uses lifecycle hooks to creates component, renders it, creates and renders its children, checks it when its data-bound properties change, and destroys it before removing it from the DOM.
Directives do have same sets of Lifecycle hooks.
There are basically 8 lifecycle hooks :

lifecycle hooks | Purpose and Timing 
--- | ---
ngOnChanges | This method respond when angular set or reset data-bound input properties. It triggers everytime whenever one or more data-bound input properties changes.
ngOnInit |  


---
### How would you share a component in other components?

---
### How to load 5GB of data efficiently on Browser?



---
### Features of reactive rxjs.



---
### How can you achieve 10min loading of Page to 2m loading of Page - stream of Data?

---
### Services are Singleton and you can share data 

throughout the code. How can you avoid this situation?
Right, if Services are imported in AppModule as provider then you can share them throughout the code. Whereas if you import them in as individual provider for each component then the share data will be confined to that particular component.

---
### How you build your app using AOT?
`ng build --aot`

---
### What build tool you use for angular?
Webpack

---
### Have you worked with video Streaming?


---
### What are Interceptors in Angular and have you used them?


---
### What code have you done which makes you proud?

...Providers and factories

> - custom theme based on angular material.
> - Authentication before loading of angular code or modules

---
### Difference between httpOptions and httpParameters?

---
### list down all the ways of communication between child and grand parent component?

> - @Output / EventEmitter
> - Subjects VS BehaviourSubject

---
### have you worked with Angular universal?


---
### ViewChildren, ContentChild, ContentChildren, and QueryList in Angular
@ViewChildren —
Returns the specified elements or directives from the view DOM as QueryList

`ViewChildren` don’t include elements that exist within the `ng-content` tag.

`ContentChildren` includes only elements that exists within the `ng-content` tag.

@ContentChildren —
Returns the specified elements or directives from the content DOM as QueryList

Remember —
The QueryList is initialized only before the ngAfterContentInit lifecycle hook, therefore, is available only from this point.

> Ref: [Medium](https://netbasal.com/understanding-viewchildren-contentchildren-and-querylist-in-angular-896b0c689f6e)

---
### How do you optimize angular build?



---
### How do you optimize frontend for performance?



---
### Explain zone.js in angular 



---
### Explain Change Detection in angular 



---
### How to you cancel Observable in angular?


...In Component, Observable gets activated only when we Subscribe to it. So unSubscribing the Subscription using unsubscribe() method will cancel the Observable.

---
### Error handling in angular




---
### How do you pass the data between components


---
### List of most commonly used operators/methods of Observable


---
### Cold Vs Hot Observables and how to make a Observable Hot?

---
### Have you ever used external Routing libraries or External Router in angular


---
### What kind of Design Pattern Angular Follows?

---
### OnPush Change Detection Strategy

---
### Difference between Angular 1 and angular 2

  




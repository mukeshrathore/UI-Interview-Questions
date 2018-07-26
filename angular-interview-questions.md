# Angular Interview Questions

### Difference between a Component and Directive?

```
Basically there are three types of directives in angular according to documentation:
- Attribute Directive -- ngStyle used to give custom behaviour to the existing elements by applying some functions/logics.
- Structural Directive -- *ngIf, *ngFor changes the DOM layout by adding and removing DOM elements. 
- Components -- These are directives with Template, Styles and Logic part. 

Component extends Directive. In this type of directive, you can use other directives whether it is custom or builtin.

```
> Reference: [Stackoverflow](https://stackoverflow.com/a/34616190)


### Difference between a Pipe and Directive?
Pipe is to manipulate data, while a directive is used for DOM manipulation.
A pipe gets data as an input, transforms it and outputs this data in another way.
A directive gets a DOM element it's "attached" to and enhances it with some kind of features.

### How can you make 2 bundles for deploying on 2 different servers while making webpack bundling?

### Difference between AOT and JIT?

### Difference Between Observable and Promise?

### Difference Between Observable and Subject?
> Reference: [Stackoverflow](https://stackoverflow.com/a/40231605)

### Explain Bootstrapping Process in Angular

### what are Life cycle hooks?

### How would you share a component in other components?

### How to load 5GB of data efficiently on Browser?

### Features of reactive rxjs.

### How can you achieve 10min loading of Page to 2m loading of Page - stream of Data?

### Services are Singleton and you can share data throughout the code. How can you avoid this situation?
Right, if Services are imported in AppModule as provider then you can share them throughout the code. Whereas if you import them in as individual provider for each component then the share data will be confined to that particular component.

### How you build your app using AOT. Hint - --aot Flag?

### What build tool you use for angular?
Webpack.

### Have you worked with video Streaming?


### What are Interceptors in Angular and have you used them?

### What code have you done which makes you proud?...Providers and factories

> - custom theme based on angular material.
> - Authentication before loading of angular code or modules

### Difference between httpOptions and httpParameters?

### list down all the ways of communication between child and grand parent component?

> - @Output 
> - Subjects VS BehaviourSubject

### have you worked with Angular universal?

### content child vs content Children






# Lesson 2 - Angular 4 Fundamentals

## Introduction
- Read through Angular documentation on [Architecture](https://angular.io/guide/architecture) 

## Fundamental building blocks of Angular application 
- From the same [Architecture](https://angular.io/guide/architecture#wrap-up) page 
- [Modules](https://angular.io/guide/architecture#modules) - An Angular app is made up of 1 or more Modules, at least 1 "root" Module. A Module is a generally a self-contained feature, a reusable piece of functionality eg: a calendar widget 
- [Components](https://angular.io/guide/architecture#components) - A Component controls a patch of screen called a *view*, by defining the template (html and angular directives) for that view, and the interactions of data and events in that view. 
- [Templates](https://angular.io/guide/architecture#templates) - A template is a form of HTML that tells Angular how to render the component. Templates use regular HTML as well as Angular [template syntax](https://angular.io/guide/template-syntax)
- [Metadata](https://angular.io/guide/architecture#metadata) - Metadata tells Angular how to process a class. Metadata is Angular defined decorators like [@Component](https://angular.io/api/core/Component) and [@Directive](https://angular.io/api/core/Directive) which inform Angular about the function(s) our ES6 classes are performing in the app/module.
- [Data binding](https://angular.io/guide/architecture#data-binding) - Data Binding "binds" the data from our class with the appropriate bindings in our templates (HTML/DOM). There are 4 types of data binding between data and our DOM, please see the diagram in the link!
- [Directives](https://angular.io/guide/architecture#directives) - A Directive defines a way of transforming template syntax / mark-up by a set of rules and functions for how that syntax should behave. eg: in the [example template](https://angular.io/guide/architecture#templates) we see Directives for [\*ngFor](https://angular.io/api/common/NgForOf) and [\*ngIf](https://angular.io/api/common/NgIf) 
- [Services](https://angular.io/guide/architecture#services) - Services provide values, functions or features to your Components and Modules. eg: logging service, database service, http request service 
- [Dependency injection](https://angular.io/guide/architecture#dependency-injection) - Dependency Injection is the process of providing your dependencies to your Angular app modules and components so that they are not hard-coded into your component but can be interchanged more easily or even mocked out for testing purposes. 

## Create Angular app and component with the CLI 
- 

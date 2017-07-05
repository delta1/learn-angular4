# Services 

- Services are one of our core building blocks in Angular apps 
- Use them to provide functionality to many components instead of duplicating code eg: database access 
- Follow the code repo: [https://github.com/delta1/ng4-tutorial](https://github.com/delta1/ng4-tutorial)

## Using Services
- To use a service it must be: 
1. Imported in the App module
2. Added to the ```providers``` array in the App module
3. Imported in the Component where you want to use it
4. Added as a parameter to the ```constructer``` function of your component class

- The service can then be used as a variable of your component class

### Example: Extend our Counter to use Local Storage 
- Goal: add a storage mechanism to our counter, to store our counter across sessions
- How?: we could use a [Document.cookie](https://developer.mozilla.org/en-US/docs/Web/API/Document/cookie), but all the cool kids use [window.localStorage](https://developer.mozilla.org/en/docs/Web/API/Window/localStorage) now (HTML5!)
- [Pros and Cons of localStorage, cookies etc](https://stackoverflow.com/a/44358718)
- We don't want to reinvent the wheel, so we google for an Angular localStorage service...
- et voilà! [https://github.com/PillowPillow/ng2-webstorage](https://github.com/PillowPillow/ng2-webstorage)
- To use it, we first need to install it from npm/yarn 
- ```yarn add ngx-webstorage```
- Import it into the app module and add it to providers
- Import it into our counter component
- Add it to the constructor of our component 
- Update the initial value of the counter to use the storage 
- Update the increment function to save our newest counter value
- Test that it works by refreshing the page! Or even close the tab and open a new one
- You can view localStorage contents in the developer tools under Application > Local Storage > URL (useful for debugging!)


## Creating Services 
- We can create our own new service using the ng cli 
- Goal: create a "randomService" which will have a function to return a random integer between 0 and 10 
- How?
- Create the new service
- ```ng generate service random```
- Import the RandomService into App module and add it to providers
- Import the RandomService into our Counter component and add it to the constructor 
- Write a function in the service to return a random integer between 0 and 10 
- Add a random button and function on our Counter component 
- Clicking the random button should call the random function, which should update the counter value and increment value with random numbers 






# What is  Redux 

 * It is a cross-platform and open-source library and has taken its inspiration from Facebook’s Flux architecture.

 * The main feature of redux is to manage and update the state of the components in an application .

##### Redux uses three main components 

1. Store - used to store state of the  component globally .

2. Action -  An action is an event that occurs when an application state is changed and sent to the redux store.
3. Reducer  - Reducers are pure functions that take the current state of the application, perform an action and return a new state.


## When to use Redux 

 Redux is needed when your application grows and maintaining the app's state becomes difficult .

 * redux is also used when the application state is changing frequently


## Advantages of Using Redux

1. Redux is Maintainable 
2. Debugging iseasy
3. Performance Benefits  
4. Ease of testing
5. Server Side Rendering 

## Drawbacks of Redux 

1. Increaded complexity 
2. Time Consuming 
3. Lack of Encapsulation
4. Excessive memory use - As the state is immutable (const) therefore when a state is updated, every time the reducer has to return a new state which leads to excessive memory usage in the long run. 


 
## React Life Cycle: 

**Mounting:** 
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase.
Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.


**Updating:**
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
static getDerivedStateFromProps, shouldComponentUpdate, render, getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

**Unmounting**
The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase

-	**constructor()**
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance.

-	static getDerivedStateFromProps()
This method exists for rare cases where the state relies on changes in props over time.

-	**render()**
Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false. Here

-	**componentDidMount()**
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

-	**shouldComponentUpdate()**
The default behavior in react is to rerender after every state change. Setting shouldComponentUpdate() to false allows you to prevent this from happening. This is in order to optimize performance. If you want to use this method, it may be better to use PureComponent instead, which performs a shallow comparison of props and state. If you do decide to use this method, be sure to check the previous props and state with the current props and state. If shouldComponentUpdate() returns false, then UNSAFE_componentWillUpdate(), render(), and componentDidUpdate() will not be invoked.

-	**getSnapshotBeforeUpdate()**
This is another rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.

-	**componentDidUpdate()**
This method is useful for performing network requests after a change has occurred.

-	**componentWillUnmount()**
This method allows you to clean up the DOM and netwrok requests/ subscriptions.

Q1) Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?<br>
 According to the order of the process in Mounting the render occurs before the componentDidMount

Q2) What is the very first thing to happen in the lifecycle of React?<br>
creating constructor

Q3) Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates? <br>
Constructor, render, componentDidMount, React Updates, componentWillUnmount

Q4) What does componentDidMount do?<br>
To load anything using a network request or initialize the DOM, it should go to componentDidMount()
 


## React State Vs Props

**Props**: are like arguments to functions, props pass into a component which means It is handled outside the component and must be updated outside the component 


State: something inside a component, is handled inside the component and must be updated inside the component 


Q1) What types of things can you pass in the props?<br>
The props can be anything from integers over objects to arrays.

Q2) What is the big difference between props and state?<br>
Props: are like arguments to functions, props pass into a component which means It is handled outside the component and must be updated outside the component 
State: something inside a component, is handled inside the component and must be updated inside the component 

Q3) When do we re-render our application?<br>
When the use makes change.

Q4) What are some examples of things that we could store in state?<br>
Numbers, strings...etc


Resourses:

- [React Life Cycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

- [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

- [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

- [React Docs - handling events](https://reactjs.org/docs/handling-events.html)




# Passing Functions as Props

![](https://scriptverse.academy/img/tutorials/reactjs-props-to-functional-component.png)
![](https://www.freecodecamp.org/news/content/images/size/w2000/2021/03/javascript-map-function.png)
- What does .map() return?  
a list of items (Array);
- If I want to loop through an array and display each value in JSX, how do I do that in React?  
use map method and wrap each value with a jsx tag.
- Each list item needs a unique key.
- What is the purpose of a key?  
they help react identify which values has been changed add or removed.  
  
Approaching the end of my journey at Flatiron School, one of the more interesting and hard subjects to learn was React. After learning pure vanilla JavaScript and being able to write an application with it, we learned the capabilities of react and how useful it is as a framework. With the transition to react, we are introduced to JSX, which is an implementation of both JavaScript and html all in one. One of the hardest things about the transition was the general use of the framework. In JavaScript, we had separate files for html and javascript. Whereas now, it’s all JSX and multiple components of an application. We are introduced to state and props, and the component lifecycle. Creating functions and making them work with state was a challenging part of the learning curve. I had a problem in a project where in the child component, I had an onClick function, and I needed that onClick function where state was, which was in the parent component. I got stuck on how to pass my function down from the parent component to the child component. When I was doing research on how to pass down functions as props into different components, I saw a lack of information on the web. So I decided to write this blog in case anyone else feels confused in this part of the React learning process.

Creating Functions at the State Level Components
When working with state, we typically want state to be in only 1 component. In other terms, we want the lowest number of components with state as possible. This means that in order to change state in a different component, we have to pass down our functions as props to the component that needs to change state. This way, we can have functions in our child components that are able to change state. This is very useful for cases where you have a child component that has an onClick function or an onChange function that needs to change state in order for the user to see the correct information on the screen.

Passing Down Functions As Props
The process of passing down functions as props can be very confusing. It happens during the render, where you call a new component. During that component call, you pass in your function as a prop. In my demonstration, I pass in the prop as [How to Pass Functions as Props](https://dev.to/vadims4/passing-down-functions-in-react-4618) .





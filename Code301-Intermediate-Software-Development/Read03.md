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
  
- What is the spread operator?  
{...}
- List 4 things that the spread operator can do.  
seperate arrays values, add arrays, seperat assignment binding.
- Give an example of using the spread operator to combine two arrays.
`let arr1 = [c,v,b]`  
`let arr2 = [d,g,h]`  
`let arr3 = [...arr1,...arr2]`
- Give an example of using the spread operator to add a new item to an array.
`let arr4=[...arr2,item]`
- Give an example of using the spread operator to combine two objects into one.
`{...objectOne, ...objectTwo}`

- In the video, what is the first step that the developer does to pass functions between components?  
create the function in the parent component.
- In your own words, what does the increment function do?  
changes the state of the parent component by being passed as props to the child component and being called there.
- How can you pass a method from a parent component into a child component?  
like a normal prop.
- How does the child component invoke a method that was passed to it from a parent component?  
simply calling it using this.methond name


## [How to Pass Functions as Props](https://dev.to/vadims4/passing-down-functions-in-react-4618)


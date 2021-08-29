# Introduction
React.js is an Open Source library developed by Facebook Developers, for building User Interfaces (UI). React makes user interfaces very easy to build by cutting each page into pieces. We call these pieces **components**.

![](https://miro.medium.com/max/700/0*5vEroMcVEXF1ghUi.jpg)


React is fairly easy to understand and at this moment has an excellent reputation and a great community. It supports [ES6](#ES6) and can perform [client-side as well as server-side rendering](#CSSR).



### Virtual DOM

![](https://www.cronj.com/blog/wp-content/uploads/DOM2.png)

Consider a page displaying a list containing 10 items and one is getting updated. [DOM](#DOM) will rebuild the entire list making it work 10 times more than what is necessary.

Virtual DOM is an abstract, lightweight copy of DOM. It can be changed as and when we want and then can be saved to the real DOM. Whenever a change occurs, Virtual DOM efficiently rerenders the DOM. It is much faster than DOM. It has the same properties as a real DOM object.





### What is a React Component?
Javascript function/class that represents a piece of a webpage. To build a page, we call these functions/classes in a certain order, put the result together, and show it to the user.


##### Function component

![](https://res.cloudinary.com/practicaldev/image/fetch/s--gVlkQ3ew--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/efvl5amf9yqhquvwvx6k.png)

##### Class component

![](https://miro.medium.com/max/932/1*1Yn5jt1VZatgx8q9uz8zJA.png)

-----

### Props
Inputs accepted by components.

![](https://s1.o7planning.com/en/12125/images/25128970.png)



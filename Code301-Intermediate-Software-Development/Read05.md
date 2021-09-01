## How would you break a mock into a component heirarchy?
The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names.

## What is the single responsibility principle and how does it apply to components?
(SRP) is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part.

## What does it mean to build a ‘static’ version of your application?
Static applications and websites render in the user's browser without the need for server side processing, this means that all the rendering of HTML, CSS, and JavaScript is done on the client side, rather then relying on server side technologies

## Once you have a static application, what do you need to add?
you’ll have a library of reusable components that render your data model. The components will only have render() methods since this is a static version of your app. The component at the top of the hierarchy (FilterableProductTable) will take your data model as a prop. If you make a change to your underlying data model and call ReactDOM.render() again, the UI will be updated. You can see how your UI is updated and where to make changes. React’s one-way data flow (also called one-way binding) keeps everything modular and fast.

## What are the three questions you can ask to determine if something is state?
1- if you want to control the behavior of the component
-2 some information that may change over the lifetime of the component
-3 change something inside Component
## How can you identify where state needs to live?
Once you've identified data, it should be stated in the application. We need to work out which components rely on the state,

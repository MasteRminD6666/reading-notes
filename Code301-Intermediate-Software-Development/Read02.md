# State
![](https://ihatetomatoes.net/wp-content/uploads/2017/09/04-react-state-vs-react-view-1024x639.jpg)
The state is an updatable structure that is used to contain data or information about the component and can change over time. The change in state can happen as a response to user action or system event. It is the heart of the react component which determines the behavior of the component and how it will render. A state must be kept as simple as possible. It represents the component's local state or information. It can only be accessed or modified inside the component or by the component directly.

# Props
![](https://miro.medium.com/max/1400/1*jWUtyVDYsZAuBhDdg4csIw.png)
Props are read-only components. It is an object which stores the value of attributes of a tag and work similar to the HTML attributes. It allows passing data from one component to other components. It is similar to function arguments and can be passed to the component the same way as arguments passed in a function. Props are immutable so we cannot modify the props from inside the component.

Difference between State and Props
SN	Props	State
1.	Props are read-only.	State changes can be asynchronous.
2.	Props are immutable.	State is mutable.
3.	Props allow you to pass data from one component to other components as an argument.	State holds information about the components.
4.	Props can be accessed by the child component.	State cannot be accessed by child components.
5.	Props are used to communicate between components.	States can be used for rendering dynamic changes with the component.
6.	Stateless component can have Props.	Stateless components cannot have State.
7.	Props make components reusable.	State cannot make components reusable.
8.	Props are external and controlled by whatever renders the component.	The State is internal and controlled by the React Component itself.
The below table will guide you about the changing in props and state.

SN	Condition	Props	State
1.	Can get initial value from parent Component?	Yes	Yes
2.	Can be changed by parent Component?	Yes	No
3.	Can set default values inside Component?	Yes	Yes
4.	Can change inside Component?	No	Yes
5.	Can set initial value for child Components?	Yes	Yes
6.	Can change in child Components?	Yes	No

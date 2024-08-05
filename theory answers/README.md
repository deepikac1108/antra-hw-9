# antra-hw-9
### Advanced Training: Assignment 9

**When should you split a component into subcomponents?**
Split a component into subcomponents when it becomes too large or complex. Also, if you find parts of the component that can be reused elsewhere, it's a good idea to split those out as well.

**What is the difference between state and props?**
- **State**: This is data that is managed within the component and can change over time.
- **Props**: These are passed to the component from its parent and cannot be changed by the component itself.

**How do you trigger a rerender in a component?**
To trigger a rerender, you can change the state or props of the component. When either of these changes, React will rerender the component to reflect the updates.

**Why do you prefer React over other front-end libraries and frameworks?**
I like React because it's fast and reactive. Its use of the Virtual DOM enhances performance, and it makes creating interactive UIs straightforward and efficient.

**What’s the difference between controlled components and uncontrolled components?**
- **Controlled components**: React manages the form data.
- **Uncontrolled components**: The DOM itself manages the form data.

**How do you prevent components from unnecessary rerendering?**
You can prevent unnecessary rerendering by using `React.memo`, `shouldComponentUpdate`, or `PureComponent`.

**Why should props be immutable?**
Props should be immutable to keep components predictable and avoid unexpected side effects, which helps maintain stability and consistency in your app.

**Explain the Virtual DOM and how React uses it to improve performance.**
The Virtual DOM is a lightweight copy of the actual DOM. React updates the Virtual DOM first and then compares it with the real DOM. It only makes the necessary updates to the real DOM, which enhances performance by minimizing direct manipulations.

**Can you explain the useMemo and useCallback hooks and provide examples of when you might use them?**
- **useMemo**: This hook caches the result of a computation, preventing it from being recalculated on every render. Use it when you have a costly computation that shouldn’t run unless its dependencies change.
- **useCallback**: This hook caches a function, ensuring the same function instance is used across renders. It’s useful when passing functions as props to child components to prevent unnecessary re-renders.

**Explain the concept of Higher-Order Components (HOCs) and provide an example use case.**
Higher-Order Components (HOCs) are functions that take a component and return a new component with added props or behavior. For example, you might use an HOC to handle authentication, wrapping a component to provide user authentication logic without altering the component itself.

**Discuss the differences between React's class components and functional components. Which one do you prefer and why?**
- **Class Components**: Use the class syntax and have access to state and lifecycle methods.
- **Functional Components**: Use functions and hooks to manage state and lifecycle.
I prefer functional components because they are simpler and, with hooks, they are just as powerful as class components.

**How do you ensure your code is maintainable and scalable?**
To ensure code maintainability and scalability:
- Write clean and modular code.
- Use meaningful variable and function names.
- Follow best practices and coding standards.
- Write tests to catch bugs early.
- Document your code to make it understandable for others and for future you.

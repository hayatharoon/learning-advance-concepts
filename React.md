# React Concepts:

## **What is React and How does it different from ohter javasrcipt framework?**

Actually React is not a framework. It is an library which is using for building user interfaces.

Here are some key aspects that differentiate React from other JavaScript frameworks:

1. **Virtual DOM:**
   React utilizes a virtual DOM, an in-memory representation of the actual browser DOM. When the state of a component change, React create a new virtual DOM representation and compare it with the previous one. Virtual DOM concept is for performance increasing.

2. **View Oriented:**
   React primarily concered with the view layer of an application. It provides a declarative way to build UI components and manages the rendering of those component efficiently.
   In React, the UI is broken into smaller, reusable components. Each component represent a specific part of the user interface and encapsulates its own logic and state. These components can be composed and nested together to form more complex UI structure.

3. **Uni-directional flow:**
   React follows a uni-directional data flow, where data flows in a single direction from parent component to child components. This promotes a predictable and easier-to-manage data flow and helps in debugging and understanding application's state.

4. **Component-based:**
   React encourages a component-based architecture, where UIs are broken down into modular and reusable components. Component can be composed and nested to create complex UI structures.

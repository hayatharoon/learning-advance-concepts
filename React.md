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

## **What is the purpose of React's Virtual DOM ?**

The purpose of React virtual DOM is to provides a performant and efficient way to update and render the user interface(UI) of a React application.
DOM is the representation of the HTML structure on a web page, and manipulating the DOM directly can be expensive. When a change occurs in a React component, instead of immediately updating the actual DOM, React updates a lightweight copy of the DOM called Virtual DOM.

### **How Virtual DOM works:**

**Initial Rendering:**
When a React component is initially rendered, React creates a representation of the component's UI in the form of a virtual DOM tree mirrors the structure of actual DOM.

**Reconciliation:**
When a component state or props change, React performs a process called reconiliation. It compares the previous Virtual DOM tree with new one generated from the updated state and props.

**Diffing and Patching:**
During the reconciliation process, React efficiently determines the minimal number of changes needed to updates the actual DOM. It performs a diffing algorithm to identify the difference (`diffing`) between the previous and new Virtual DOM trees.

**Updating the Actual DOM:**
Once the diffing is identied, React applies the necessary changes to the actual DOM, It updates only the parts of DOM that have changed, minimizing the amount of manipulation required.

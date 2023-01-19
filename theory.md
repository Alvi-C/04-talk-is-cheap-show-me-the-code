1.  Is JSX mandatory for React?
    A. No, JSX is a way of creating UI components, which makes our work more easier in comparison to React.createElemet.

2.  Is ES6 mandatory for React?
    A. No, ES6 is enhanced version of javascript which include map, const, spread operator, destructuring and many more. Which at the end achive the requrement with less code and in much optimize way.

3.  How can i write comment in JSX?
    A. Block comment {/\* \*/}

4.  What is <React.Fragment></React.Fragment> and <></>?
    A. In React, a fragment is a way to group a list of children without adding extra nodes to the DOM. A fragment is represented by using the special <React.Fragment> or <> (short syntax) JSX tags. It allows you to return multiple elements from a component's render method without adding an extra parent element to the DOM.

5.  What is Virtual DOM?
    A. The Virtual DOM is a programming concept used in JavaScript libraries and frameworks, such as React, to optimize the performance of web applications. It works by keeping a virtual representation of the actual DOM (Document Object Model) in memory, and only updating the parts of the real DOM that have changed. This allows for faster updates and smoother user interactions, as the browser does not need to re-render the entire page.

6.  What is Reconciliation in react?
    A. Reconciliation is the process that React uses to determine what changes need to be made to the actual DOM, based on the updates made to the virtual DOM. When a component's state or props change, React will compare the current virtual DOM with the new virtual DOM and determine the minimal set of changes needed to bring the actual DOM into alignment with the new virtual DOM. These changes are then made to the actual DOM, resulting in the update of the rendered component. This process is efficient and fast due to the use of the virtual DOM.

7.  What is React Fibre?
    A. React Fiber is a new reconciliation algorithm introduced in React 16. It is a complete rewrite of the previous algorithm, designed to increase the flexibility and performance of React.

8.  Why do we need Key in react? When do we need key in react?
    A. Key is used to uniquely identify our react elements so that the reconciliation can easily find the new added element and only re-render that elements intead of re-rendering all the similar elements. We need Key in react when we have multiple elements of same html tag.

9.  Can we use index as key in react?
    A. No we should not use index as a key in react, if the order of items may change. This can negatively impact performance and may cause issues with component state. If ther is no unique code available then in that case we can use index as a key in react.

10. What is props in react?
    A. In react every components at the end is javascript function so we can pass arguments as the parameters into any functional components
    are called props.
    Ex.
    const PassAttributeComponent = (props) => {
    return (<div style={props.style} key={props.key}>
    {props.children}</div>)
    }

    const DisplayAllElements = () => {
    return (
    <div>
        <PassAttributeComponent style={{ color: "red" }} key="05">Hello I am children </PassAttributeComponent>
    </div>)
    }

11. What is config driven UI?
    A. A config-driven UI refers to the approach of building user interfaces where the layout, behavior and appearance of the components are determined by a configuration file rather than hard-coded into the application's source code.

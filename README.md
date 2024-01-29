# DEVELOPER HANDBOOK

### React Developer Roadmap (2024)

A thorough React developer roadmap for 2024 that addresses all aspects of React and beyond.

<details>

<summary>0. Before you start React</summary>

You should know and be comfortable with **all of the following:**

-   [**Basic HTML**](https://www.w3schools.com/html/default.asp)

    -   HTML Elements, Attributes, Headings, Paragraphs, Colors & Styles
    -   HTML Links, Images, Tables, Lists, Block & Inline, Div, Classes, Id
    -   HTML Forms
    -   HTML Layout, Responsiveness & Semantic

-   [**Basic CSS**](https://www.w3schools.com/css/default.asp)

    -   CSS Basics - Syntax, Selectors, Colors, Backgrounds, Borders, Margin, Padding, Height/Width, Box Model, Outline, Text, Fonts, Links etc.
    -   CSS More - Lists, Tables, Display, Position, z-index, Overflow, Float, Inline Block, Align, Combinators, Pseudo-classes & elements, Opacity etc.
    -   CSS Forms & Layouts
    -   CSS Flexbox
    -   CSS Grid
    -   Advanced CSS - CSS Units, Shadows, Gradients, Transitions, Animations, Specificity etc.

-   [**Basic Tailwind CSS**](https://www.youtube.com/watch?v=X7XbjwD6fVY&list=PLHiZ4m8vCp9P23SqlHL0QAqiwS_oCofV2)

    -   Tailwind Utilities
    -   Responsive Variants
    -   Hover, focus and other states
    -   Dark Mode variant
    -   Tailwind Directives
    -   Tailwind Configurations
    -   Theme Configurations
    -   [Tailwind cn() utility](https://www.youtube.com/watch?v=y7DrXkGj7AU)

-   **Document Object Model (DOM)**

    -   [DOM Basics - Basics, Method, Document, Elements, Forms, CSS, Events, Navigation, Nodes and Collections](https://www.youtube.com/watch?v=mPTkKnL2aNA&list=PLHiZ4m8vCp9OkrURufHpGUUTBjJhO9Ghy)
    -   [DOM Advanced](https://www.youtube.com/watch?v=XY96d0vEdFk&list=PLHiZ4m8vCp9MJDxMOzhYVuTrO1b5n-Tq_)

-   [**Basic JavaScript**](https://www.youtube.com/watch?v=rePN-VFo1Eo&list=PLHiZ4m8vCp9OkrURufHpGUUTBjJhO9Ghy)

    -   JS Basics - Statements, Expressions, Syntax, Variables, Operators, Data Types, Functions, Objects, Arrays, Events, Array and String Methods, Object Methods, Date, Conditionals, Error Handling, JavaScript OOP - classes and inheritance and Debugging
    -   JS Web APIs - Forms, History, Geolocation, Storage, Worker and Fetch API
    -   JS JSON

-   [**JavaScript Advanced**](https://www.youtube.com/watch?v=KuhLGuNxF8U&list=PLHiZ4m8vCp9Nflbo9a0pZuLscG_Xc7DKq)

    -   Solid JS Concepts - Scope, Hosting, Execution Context, Closures, Prototype, Recursion, Primitive vs Reference Data Types, Currying, Intersection Observer, Memoization, Event Propagation, Debounce etc.
    -   [Asynchronous JavaScript](https://www.youtube.com/watch?v=IUBd76UQb34) - Callbacks, Promises and async-await

-   [**Modern JavaScript**](https://www.youtube.com/watch?v=PWXkYBmlbB4&list=PLHiZ4m8vCp9MFjMRp9EEHWKArbi0wdgXG)

    -   Different ES6+ JS Syntaxes and concepts eg. Arrow function, Truthy/Falsy values, Ternary Operator, Different Array methods like find, filter, map, reduce, slice, splice, push, pop, concat, different looping strategies, Spread & Rest Operator, Array and Object Destructuring, Imports/Exports syntax, Template Literals, Sorting etc.

-   [**Git/GitHub**](https://www.youtube.com/watch?v=PWXkYBmlbB4&list=PLHiZ4m8vCp9MFjMRp9EEHWKArbi0wdgXG)

    -   [Basics of Git](https://www.youtube.com/watch?v=oe21Nlq8GS4)
    -   [Important Git Commands](https://learnwithsumit.com/rnext/courses/rnext/git-github-refresher)

</details>

<details>
<summary>1. React Fundamentals</summary>

You should know and be comfortable with **all of the following:**

-   **Getting Started with React**
    -   Introduction to React - Why React - Comparison with Vanilla JS
    -   React Installation & Editor Setup with Vite
    -   How React works - Virtual DOM
    -   Basics of React Components
    -   Basics of JSX: React's Markup
    -   JavaScript in JSX
    -   Passing Props to Components
    -   Conditional Rendering
    -   Rendering Lists
    -   Pure Components
    -   How to split larger components into smaller ones
-   **Adding Interactivity**

    -   Responding to Events - Event Handlers
    -   Understanding States - React Component's Memory - useState
    -   How State works in React
    -   How Rendering works in React
    -   Updating complex states immutably in React

-   **React State Management Deep Dive**

    -   Declarative vs Imperative UI
    -   Thinking UI Declaratively
    -   Finding & Structuring React States
    -   Connecting Event Handlers to React
    -   Sharing State between components
    -   Lifting State up
    -   Extracting State Logic into Reducers
    -   useReducer Hook
    -   How to use Immer with React for concised immutable State Update
    -   Passing Data Deeply inside React Components
    -   Avoiding Prop Drilling - Context API & useContext Hook
    -   Combine context and reducer to write scalable code

</details>

<details>
<summary>2. Advanced React</summary>

-   Referencing values with Refs - useRef hook
-   Manipulating the DOM with Refs
-   Synchronizing with Effects - useEffect hook
-   Separating events from Effects
-   Removing Effect Dependencies
-   Performance optimization with useCallback and useMemo hook
-   Reusing logic with Custom Hooks
-   Calling APIs from Back-end with React

</details>

<details>
<summary>3. Advanced State Management</summary>

##### [Using Redux / Toolkit](https://learnwithsumit.com/think-in-a-redux-way)

-   ##### Redux

-   ##### Redux Thunk

    -   ###### What is Redux Thunk
        `Redux Thunk` হলো `Redux` এর একটি `middleware` যা আমাদের এপ্লিকেশনের asyncronus টাস্ক গুলো ম্যানেজ করতে হেল্প করে । `React` এপ্লিকেশনের asyncronus টাস্ক গুলো ম্যানেজ করার জন্য `Redux Thunk` ব্যাবহার করা হয় ।
    -   ###### Using Steps of Redux Thunk

        নিচের কিছু স্টেপ ফলো করে আমরা `Redux Thunk` ব্যাবহার করতে পারি:

        -   **Step 1 : Install Redux Thunk**:

        ```bash
         npm i redux-thunk
        ```

</details>

<details>
<summary>4. Styling Solutions</summary>

-   [**Tailwind**](https://tailwindcss.com/)
-   [**CSS Modules**](https://www.makeuseof.com/react-components-css-modules-style/)
-   [**Styled Components**](https://styled-components.com/)
-   React UI Component Library - [Shadcn](https://ui.shadcn.com/)
-   [React UI Component Library - Keep React](https://youtu.be/mVXNUMBtGEA)
-   [**Material UI**](https://mui.com/)
-   [**Chakra UI**](https://chakra-ui.com/)
-   [**Ant Design**](https://ant.design/docs/react/introduce)

</details>

<details>
<summary>5. React Ecosystem & Use Cases</summary>

-   [React Router DOM](https://youtu.be/34tjWL9wi4g)
-   API Request with Axios in React
-   React Suspense & Error Boundaries
-   React Lazy Load
-   React Infinite Scroll
-   Uncommon React Hooks - useDebugValue, useDeferredValue, useId, useImperativeHandle, useInsertionEffect, useLayoutEffect and useTransition
-   **React Authentication**

    -   How to handle user sign in (email, password, JWT)
    -   How to handle access tokens and token refreshes
    -   Social sign in (Google, Facebook, GitHub, etc.)
    -   [Using Supabase](https://supabase.com/)
    -   [Using Firebase](https://firebase.google.com/docs/auth)
    -   [Using Clerk](https://clerk.com/)

-   **Form Handling in React**

    -   How to validate user input in forms (emails, passwords, etc.)
    -   How to send form data to server
    -   How to handle file uploads
    -   [Using React Hook Form](https://react-hook-form.com/)
    -   [Using Formik](https://formik.org/docs/overview)

-   [**Accessibility**](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/React_accessibility)
    -   Understanding why accessibility is important
    -   [Using semantic HTML](https://www.semrush.com/blog/semantic-html5-guide/)
    -   How to implement keyboard navigation
    -   How to add aria labels
    -   [Using React Aria](https://react-spectrum.adobe.com/react-aria/)
-   **Testing**
    -   [How to implement unit tests](https://www.freecodecamp.org/news/how-to-write-unit-tests-in-react/)
        -   [Using React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)
        -   [Using Jest](https://jestjs.io/)
    -   [How to implement e2e integration tests](https://youtu.be/6BkcHAEWeTU)
        -   [Using Cypress](https://www.cypress.io/)
        -   [Using Playwright](https://playwright.dev/)

</details>

<details>
<summary>6. React Frameworks</summary>

You should have worked with **one of the following:**

-   [**Vite**](https://vitejs.dev/)
    -   How to run a simple React application
-   [**Next.js**](https://nextjs.org/)
    -   [Understanding file-based routing](https://nextjs.org/docs/app/building-your-application/routing)
    -   [Understanding Next Auth](https://next-auth.js.org/)
    -   [Understanding server components](https://nextjs.org/docs/app/building-your-application/rendering/server-components)
    -   [Understanding server actions](https://nextjs.org/docs/app/building-your-application/data-fetching/server-actions-and-mutations)
-   [**Remix**](https://remix.run/)

</details>

<details>
<summary>7. Beyond React</summary>

-   **Team player**
    -   How to work within a team
    -   How to perform code reviews
    -   How to give and receive feedback
-   **Efficiency**
    -   How to prioritise tasks
    -   How to handle tech debt
    -   How to meet deadlines and goals
-   **Continuous Learning**
    -   How to continuously learn and grow
    -   How to stay up to date with your skills
-   **Networking & Communication** - Going to meetups or events - Contributing to open source projects - Networking within the company you work in
</details>

### How to pass data to deeply nested components in React ?

-   Props Drilling
-   Render Props
-   HOC Pattern
-   Context API
-   Redux Store Provider

-   #### Props Drilling

    -   এক কম্পোনেন্ট থেকে আরেক কম্পোনেন্ট এ `Props` আকারে ডাটা পাস করে আমরা কাজ করতে পারি। এই `Props` পাস করে করে নেস্টেট কম্পোনেন্ট গুলোতে ডাটা পাস করার টেকনিক কে বলা হয় ` Propos Drilling Technique` এই `Props Drilling` হলো `unidirectional` অর্থাৎ একমুখী ডাটা পাস করা যায়। রিয়াক্টে সবসময় `Parent Component` থেকে `Child Component` এ ডাটা পাস করা যায় ।

    যদি আমাদের কখনো `Child Component` থেকে `Parent Component` এ ডাটা পাস করার প্রয়োজন পরে তাহলে আমরা রিয়াক্টে ডাটা পাস করার অন্য আরেকটি টেকনিক `Render Props Pattern (RP Pattern)` ব্যাবহার করতে পারি ।

-   #### 1. Render Props

    -   `Render Props` হলো রিয়াক্ট এ `Child Component` থেকে `Parent Component` ডাটা পাস করার একটা টেকনিক ।

        এতে আমরা `Parent Component` এ কোন `function` লিখে তা `Props Drilling` এর মাধ্যমে `Parent Component` এ `function` রেফারেন্স টা পাস করে তার `arguments` আকারে `Child Component` থেকে ডাটা `Parent Component` এ পাস করতে পারি ।

-   #### 2. HOC Pattern

    -   ` HOC Pattern (Higher Order Components Pattern)`

-   #### 3. Context API

    -   জাভাস্ক্রিপ্ট এর `Context Api` ব্যাবহার করে `React` একটা হুক বানিয়েছে `useContext` নামে। এই হুক ব্যাবহার করে আমারা যেকোনো কম্পোনেন্ট থেকে যেকোনো কম্পোনেন্টে ডাটা পাস এবং রিসিভ করতে পারি । সেক্ষেত্রে যত ডিপলী নেস্টেট কম্পোনেন্ট থাকুক না কেন আমরা নিশ্চিন্তে এক কম্পোনেন্ট থেকে আরেক কম্পোনেন্ট এ ডাটা পাস করতে পারবো ।

-   #### 4. Redux Store Provider
    -   Redux State management Library ব্যাবহার করে আমরা ডাটা যেকোনো কম্পোনেন্ট এ পাস করতে পারি ।

### How to Manage Complex States in React

-   useReducer Hook
-   useReducer with Context
-   Redux Core
-   Redux Toolkit

রিয়াক্ট এর কমপ্লেক্স স্টেট গুলো ম্যানেজ করার জন্য বেশ কিছু টেকনিক আছে , তা হলো ঃ

#### 1. useReducer Hook

-   `useReducer` হলো রিয়ক্ট এর একটি হুক যা জাভাস্ক্রিপ্ট এর `Array.reducer()` মেথড টা ইউজ করে বানানো হয়েছে । এতে করে আমরা `React` এর কমপ্লেক্স স্টেট গুলো খুব সহজে ম্যানেজ করতে পারি । নিচে `useReducer` হুক ব্যাবহার করার স্টেপ বাই স্টেপ ইন্সট্রাকশন দেয়া হলো ঃ

ধরা যাক আমরা একটা `Counter` বানাচ্ছি ।

## ` #Step 1 :`

প্রথমে আমাদের একটা `reducer function` বানানো লাগবে যেকোনো নামে,তবে বুঝার সুবিধার জন্য `Counter` নামেই ফাংশনটা বানানো উচিত। আমারাদের কোড যেন সুন্দর থাকে, তাই আমরা ফাংশন টা একটা আলাদা ফাইলে বানাবো এবং সেখানে থেকে `function` টাকে `export` করে দিবো যাতে অন্য যেকোনো জায়গায় ফাংশনটা ব্যাবহার করতে পারি।

```javascript
//CounterReducer.js
export const counterReducer = () => {};
```

এখানে `counterReducer function` টি `parameter` হিসেবে দুইটি জিনিস নেয়,

1. state : `state` এ আমরা আমাদের স্টেট এর ভ্যালু পাই ।
2. action: `action` এ আমরা একটা অবজেক্ট পাই । এই অবজেক্ট এর `property` হিসেবে আমরা `type` আর `payload` পাই।

```javascript
//CounterReducer.js
export const counterReducer = (state, action) => {};
```

`counterReducer function` টি বিভিন্ন লজিকের বিভিন্ন `action` এর বিপরীতে `state` এর ভ্যালু আপডেট করবে । এক্ষেত্রে আমরা `switch case` ব্যাবহার করবো ।

```javascript
//CounterReducer.js
const initialValue = 0;
export const counterReducer = (state = initialValue, action) => {
    switch (action.type) {
        case "INCRIMENT": {
            return state + 1;
        }
        case "DECRIMENT": {
            return state - 1;
        }
        default: {
            return state;
        }
    }
};
```

উপরে `action` এর যেই `case` গুলো ব্যাবহার করা হয়েছে তা আমরা কম্পোনেন্ট থেকে `dispatch` করবো ।

## ` #Step 2 :`

এই স্টেপে আমরা `component` এ `reducer` এর স্টেট এর ভ্যালু ব্যাবহার করবো ।

```javascript
//Counter.jsx
 export default function Counter(){
    return <button>
        <h1> Count : 0</h1>
        <button>Incriment</button>
        <button>Decriment</button>
    </>
 }
```

উপরের `Counter component` এ আমরা `react` এর `useReducer` হুক ব্যাবহার করবো । `useReducer` হুক দুইটা টুপল `tuple` রিটার্ন করে, একটি হলো `state` এবং অপরটি হলো `dispatch` এবং হুকটি `parameter` এ দুইটি জিনিস রিসিভ করে , একটি হলো `reducerFunction` এবং অপরটি হলো `initialValue`.

`initialValue` যেকোনো টাইপের হতে পারে। যেহেতু আমরা `counter` বানাচ্ছি ,তাই আমরা `initialValue` নাম্বার দিচ্ছি ,এবং সেটা `state` এর ডিফল্ট ভ্যালু হিসেবে সেট করে দিচ্ছি ।

```javascript
//Counter.jsx
import {useReducer} from "react"
import {counterReducer} from "./reducer/CounterReducer.js"

 export default function Counter(){

 const [count,dispatch]= useReducer(counterReducer,0)

    return <button>
        <h1> Count : 0</h1>
        <button>Incriment</button>
        <button>Decriment</button>
    </>
 }
```

`count` এর ভিতর আমরা `Counter` এর স্টেট টা পাবো এবং তা `Count` এর ভ্যালু হিসেবে সেট করে দিবো ।

`button` গুলোর `onClick` হান্ডেলারে আমরা `action dispatch` করবো ।

```javascript
//Counter.jsx
import {useReducer} from "react"
import {counterReducer} from "./reducer/CounterReducer.js"

 export default function Counter(){

 const [count,dispatch]= useReducer(counterReducer,0)
    //action handler
    function handleIncrement(){
        return dispatch({type:"INCRIMENT"})
    }

     function handleDecrement(){
    return dispatch({type:"DECRIMENT"})
    }

    return <button>
        <h1> Count : {count} </h1>
        <button onClick={handleIncriment}>Incriment</button>
        <button onClick={handleDecriment}>Decriment</button>
    </>
 }
```

#### 2. Context With Reducer

## `#Step : 1`

প্রথমে আমাদের একটা `context` বানাতে হবে । সেজন্য একটা ফাইল নিব `CouterContext.js` নামে । এবং রিয়াক্টের `createContext` ব্যাবহার করে একটা `context` বানাতে হবে ।

```javascript
//counterContext.js
import { createContext } from "react";
export const counterContext = createContext(null);
```

## `#Step : 2`

`Context` এর `Provider` এর ভ্যালুতে আমারা ডাটা পাস করবো ।

```javascript
//counterContext.js
import { createContext,useReducer } from "react";
export const counterContext = createContext(null);

export default counterContextProvider({children}){

 const [count,dispatch]= useReducer(counterReducer,0);
    return(
     <>
        <counterContext.Provider value = {{count,dispatch}}>
            {children}
        </counterContext.Provider>
     </>
    )
}
```

## `#Step : 3`

আমরা যেই `component` থেকে তার সকল নেস্টেট `ChildComponent` এ ডাটা এক্সেস করতে চাইবো সেই `component` কে আমরা `contextProvider` দিয়ে wrap করে দিবো ।

```javascript
//Main.jsx
import CounterContextProvider from "../context/counterContext";
<CounterContextProvider>
    <App />
</CounterContextProvider>;
```

## `#Step : 4`

এবার আমারা যেই `component ` এ ভ্যালু এক্সেস করতে চাইবো সেখান থেকে শুধু `context` এর মাধ্যমে ডাটা রিসিভ করে বিভিন্ন `action dispatch` করতে পারবো ।

```javascript
//Counter.jsx
 export default function Counter(){
    const {count,dispatch} = useContext(couterContext)
    //action handler
    function handleIncrement(){
        return dispatch({type:"INCRIMENT"})
    }

     function handleDecrement(){
    return dispatch({type:"DECRIMENT"})
    }

    return <button>
        <h1> Count : {count} </h1>
        <button onClick={handleIncriment}>Incriment</button>
        <button onClick={handleDecriment}>Decriment</button>
    </>
 }
```

#### 3. Redux Core

#### 4. Redux Toolkit


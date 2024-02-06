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

-   ## **Getting Started with React**

    -   #### Introduction to React - Why React - Comparison with Vanilla JS

        <blockquote><i>React is a javascript library which is created for building web and native user interfaces. In 2011 a facebook engineer named “JORDAN WALKE” created React js . he was inspired by a php library called XHP-JS. React was first used in facebook timeline in 2011 and then 2012 used in Instagram. Though it is very affective,that’s why facebook makes it a opensource for all.</i></blockquote>

         <blockquote><i>In vanila javascript  after a user interaction UI have to change manualy,In a large project which is a very costly and difficult to maintain. **Facebook** also face this problem as well.thats why they think seriously and create React js. React helps us to get rid of this problem. **In a react application when user interact,and after user interaction we just need to change the data or state,react automaticaly change the UI. we don’t need to change the UI manualy. this is the main beauty of React. and also react’s each component have independent State. which means , Every component and its states are separate.**
        Lets think an example:

        This is a simple product card. And we have a task that “ when a user click on Add to cart button ,the total price will multiply the price according to the click count. Which means If a user click Add to card button once total price should be 6000 and if click twice,the total price will be 12000 and so on.."

        pretty simple task write?

        **Lets do it with vanila javascript firtst:**

        1. We have to select all the HTML DOM Element. then
        2. We have to set initial state of product price and total price.then
        3. We have to render the initial state value to HTML DOM. then
        4. We have to update the state value with the user click interaction on **Add to cart** button. then
        5. **We have to update dom manualy to see the DOM CHANGES.**

        Pretty simple task for now , write??.. Wait.. If we have to do this with 10/20/100 products ?

        OOHH ! we have to do the same thing again and again.

        So, this process is not a easy way and every time after change any value it need to update the DOM manualy,which is really very costly and very hard to maintain in a large scale application.

        That’s why React comes to play.

        **Lets do this again with React:**

        **What we have to do with react? let’s see…**

        We have a simple product card UI component. and we set a initial state of product price and quantity.

        after a user click on **Add to cart Button** we just need to update our click count or Quantity state.

        And React do the rest…

        It automaticaly update the UI with the helps of **ReactDOM.** So, we don’t need to be panic to update the UI. which process is very very easy to maintain and scaling any large or any size application. Because React components state are independent. which means if we have this same product component Hundreds or Thousends.. No matter, each components has its won independent state.

        So, What we learned ?

        We learned that React is come to helps us to write code very easy and effective way and don’t need to be panic to update UI. Because this is React. React always Reactive. Its need just data change and it will do the rest by itself.\*\*</i></blockquote>

    -   #### React Installation & Editor Setup with Vite

         <blockquote>
         <i>
        React Recomment to use a framework with react. but this time we will install react with vite

        ```bash

            npm create vite@latest --template react

        ```

         </i>
         </blockquote>

    -   #### How React works - Virtual DOM

         <blockquote>

        ভার্চুয়াল ডম এর মাধমেই মুলত রিয়াক্ট কাজ করে থাকে।

        রিয়াক্ট তার পুরো ওয়েব এপ্লিকেশনকে একটা কম্পনেন্ট ট্রি আকারে চিন্তা করে, অনেকটা DOM এর মতো।

        যখন ইউজারের কোন ইন্টারেকশনের কারনে কোন একটা কম্পনেন্ট এ কিছু চেঞ্জ করা লাগে,তখনি রিয়াক্ট তার ভার্চুয়াল ডম কন্সেপ্টটাকে কাজে লাগায়।

        যখন ই কোন কম্পনেন্ট এ কিছু চেঞ্জ হয়,তখনি রিয়াক্ট তার যে মেইন কম্পোনেন্ট আছে তার মদ্ধে যেই চেঞ্জটা হলো তার ঠিক আগে কম্পোনেন্ট টা যেই অবস্থায় ছিল,সেটার একটা সেম কপি বানিয়ে ফেলে তার ভার্চুয়াল ডম অব্জেক্ট এ।

        তারপর রিয়াক্ট তার Diffing or Reconciliation এল্গরিদম এর সাহায্যে দুইটাকে পাশাপাশি তুলনা করে বুঝতে পারে যে,কম্পোনেন্ট এর ঠিক কোন জায়গায় বা কোন ইলিমেন্টে পরিবর্তন হয়েছে আর ব্রাউজার এ ঠিক কোন জায়গায় পরিবর্তন দেখাতে হবে।

        তখন ঠিক সেই জায়গায় রিয়াক্ট পুরো ডমটাকে রি রেন্ডার না করে,ঠিক যেই যায়গায় চেঞ্জ হয়েছে,ঠিক সেই জায়গায় ডমটাকে চেঞ্জ করে দেয়।

        এতে করে যেই লাভ টা হচ্ছে যে, নরমাল কোন ওয়েব এপ্লিকেশনে বার বার প্রতিটা ইন্টারেকশনে RenderTree টাকে Repaint করতে যে সময়টা লাগছে তা রিয়াক্ট এ লাগছেনা,কারন রিয়াক্ট তার reconciliation এল্গরিদম এর মাদ্ধমে একেবারে মিনিমাম চেঞ্জ করছে, এতে করে ডম ম্যানিপুলেশন কমে যাচ্ছে তাই আমরা পার্ফমেন্স টা যথেষ্ট ফাস্ট পাচ্ছি। </blockquote>

    -   #### Basics of React Components

         <blockquote>
         React applications are built from isolated pieces of UI called components. A React component is a JavaScript function that you can sprinkle with markup.

        Components can be as small as a button, or as large as an entire page.

        In a React app, every piece of UI is a component.

        React components are regular JavaScript functions ,But...

        1. Their names always begin with a capital letter.
        2. They return JSX markup.

        **Steps for defining a component**

        `Step 1:` Export the component

        `Step 2:` Define the function

        ` Step 3:` Add markup

        ```jsx
        export default function MyComponent() {
            return (
                <div>
                    <h1>This is My First Componnet</h1>
                </div>
            );
        }
        ```

        <i>Return statements can be written all on one line,But if your markup isn’t all on the same line as the return keyword, you must wrap it in a pair of parentheses.Without parentheses, any code on the lines after return will be ignored!</i>

        </blockquote>

    -   #### Importing and Exporting Components

         <blockquote>
         জাভাস্ক্রিপ্ট এ মূলত দুইভাবে `import` and `export` করা যায় ।
         
         1. Default export/import
         2. Named export/import

        **Default export/import**

        একটি ফাইল থেকে মাত্র একটি default export করা যাবে ।

        ```javascript

        //way 1 of default export
        export default function MyComponent() {
            return; // something jsx
        }


        //way 2 of default export
        const MyComponent = () => {
            return; // something jsx
        };
        export default MyComponent;

        ```

        `default exported component` ইম্পোর্ট করা যায় দুইভাবে ঃ

        ```javascript
        //Way 1 of Default Import
        import MyComponent from "./MyComponent";

        //Way 2 of Default Import
        import SomethingOtherName from "./MyComponent";
        ```

        খেয়াল করুন `default import` এর ক্ষেত্রে আমরা `Component` কে যেকোন নামে ইম্পোর্ট করতে পারি । তবে `Component` ব্যাবহার করার সময় যেই নামে ইম্পোর্ট করা হয়েছে সেই নামেই ব্যাবহার করতে হবে ।

        **Named export/import**

        একটি ফাইল থেকে একাধিক `named export` করা যায় ।

        ```javascript
        //named export
        export function MyComponent() {
            return; // something jsx
        }
        ```

        `named exported component` ইম্পোর্ট করার সময় অবশ্যই যেই নামে এক্সপোর্ট করা হয়েছে সেই নামেই ইম্পোর্ট করতে হবে এবং নামটা অবশ্যই {} এর মাঝখানে লিখতে হবে ।

        ```javascript
        //named import
        import { MyComponent } from "./MyComponent";
        ```

        `named exported component` ইম্পোর্ট করার সময় চাইলে `alias` দিয়েও ইম্পোর্ট করা যায়,সেক্ষেত্র `Component` ব্যাবহার করার সময়ও `Alias` নামেই ব্যাবহার করা লাগবে

        ```javascript
        //named import
        import { MyComponent as SomethingOtherName } from "./MyComponent";
        ```

         </blockquote>

    -   #### JavaScript in JSX

        আমরা JSX এর ভিতরে ডায়নামিক জাভাস্ক্রিপ্ট এর একপ্রেশন লিখতে পারি ।

        JSX এ জাভাস্ক্রিপ্ট একপ্রেশন লিখতে হলে আমাদেরকে তা `{}` এর ভিতরে লিখতে হবে ।

        ```javascript
        export default function TodoList() {
            const name = "Gregorio Y. Zara";
            return <h1>{name}'s To Do List</h1>;
        }
        ```

    -   #### Passing Props to Components

        React Components use props to communicate with each other. Props are like Html attributes. but main difference is - we can pass any javascript value as props like array object even function as well.

        **React Props or Data are unidirectional. It means we can only pass data/props from Parents to Child Component**

        We can pass props to a component in two simple steps:

        `Step 1:` Pass props to the child component:

        ```javascript
        export default function Profile() {
            return (
                <Avatar
                    person={{ name: "Lin Lanying", imageId: "1bX5QH6" }}
                    size={100}
                />
            );
        }
        ```

        `Step 2:` Read props inside the child component

        We can read props from child components as arguments of function.

        ```javascript
        function Avatar(props) {
            let person = props.person;
            let size = props.size;
            // ...
        }
        ```

        Usually we don’t need the whole props object itself, so we cab destructure it into individual props.

        ```javascript
        function Avatar({ person, size }) {
            // ...
        }
        ```

        This syntax is called “destructuring” and is equivalent to reading properties from a function parameter.

        **Specifying a default value for a prop**

        we can give a default value to a props as a fallback right after the props by assigning with `=` operator.

        default value will use only when the props is missing or `undefined`,but if we pass `null` or `0`,the default value will not be used.

        We can forward all props with <Avatar {...props} /> JSX spread syntax, but we shouldn't overuse it!

    -   #### Conditional Rendering

        আমরা অনেকভাবে রিয়াক্টে কন্ডিশনাল রেন্ডারিং করতে পারি ঃ

            1.  If Statement
            2.  Logical AND -`&&`
            3.  Logical OR -`||`
            4.  Ternery Operators - `? :`
            5.  Nullinsh Colasing Operators - `??`

    -   #### Rendering Lists

        জাভাস্ক্রিপ্ট এ আমাদের অনেক সময় লিস্ট আইটেম শো করানোর প্রয়োজন পরে । যদি আমাদের কোন Array ডাটা স্ট্রাকচার থাকে তখন আমাদেরকে `map` করে সেই ডাটা লিস্ট শো করাতে হয়। এখানেও আমরা Array ডাটা শো করানোর সময় `map` ব্যাবহার করবো।তবে এক্ষেত্রে আমরা লিস্ট আইটেম ম্যাপ করার সময় আইটেম কম্পোনেন্ট এ একটা ইউনিক `key={}` আইডেন্টিফায়ার ব্যাবহার করতে হবে ।

        এই `key={}` আমাদের প্রতিটা কম্পোনেন্ট কে আলাদা আলাদা করে রিপ্রেসেন্ট করে । এতে আমাদের অনেক বাগ থকে মুক্তি মেলে।

        `key={}` ব্যাবহার করার সময় আমাদের কিছু জিনিশ মাথায় রাখতে হবে ঃ

        ১। `key={}` এর ভ্যালু হিসেবে আমাদের কখনওই Array এর index ব্যাবহার করা উচিত না ।

        ২। `key={}` ব্যাবহার করার করার সময় কখনওই আমরা on the fly(ইনস্ট্যান্ট) `key` জেনারেট করে ব্যাবহার করতে পারবোনা। সবচাইতে ভালো হয় যদি আমাদের ডাটাতে কোন ইউনিক আইডেন্টিফায়ার থাকে । তাহলে সহজেই আমরা সেই আইডেন্টিফায়ার কে key হিসেবে ব্যাবহার করতে পারবো ।

    -   #### Pure Components

        আমাদের প্রতিটা কম্পোনেন্টকে `Pure Component` হিসেবে বানানো উচিত। পিউর কম্পোনেন্ট এর কিছু বৈশিষ্ট্য হলো ঃ

        ১। এটা শুধু তার নিজের কাজ করে। তার যতটুকু কাজ সে শুধু ততটুকু কাজ এ করবে । এটা বাহিরের কোন variable কে তার নিজের ভিতরে পরিবর্তন করবে না। ২। সবসময় সেম ইনপুটের সেম আঊটপুট দিবে ।

        You should not mutate any of the inputs that your components use for rendering. That includes props, state, and context. To update the screen, “set” state instead of mutating preexisting objects.

    -   #### How to split larger components into smaller ones

-   **Adding Interactivity**

    -   #### Responding to Events - Event Handlers

        আমরা রিয়াক্ট কম্পোনেন্ট গুলোতে ইউজারের বিভিন্ন ইন্টারেকশনে ইভেন্ট হেন্ডেলার বসাতে পারি । যা আমাদের UI কে ইন্টারেক্টিভ করে তুলে।

        **Event Deligation in Javascript**

        `event deligation` হলো এমন একটা টেকনিক,যা দিয়ে আমরা একটা ইভেন্ট লিসেনার দিয়ে অনেকগুলো element কে কনট্রোল করতে পারি এবং যদি আমদের আইটেম বাড়ে তাতেও আমদের event handler ঠিক কাজ করবে ।

        ধরা যাক,আমাদের একটা ডাটা লিস্ট আছে । যেমনঃ

        ```html
        <ul>
            <li>Apple</li>
            <li>Banana</li>
            <li>Orange</li>
        </ul>
        ```

        এই লিস্ট এর ডাটাগুলো সব API থেকে আসছে,এবং ভবিষ্যতে ডাটা বারতেও পারে কমতেও পারে,যা আমরা জানিনা । এখন ধরা যাক যে আমাদের লিস্ট এ আরও কিছু আইটেম চলে আসলো ,

        ```html
        <ul>
            <li>Apple</li>
            <li>Banana</li>
            <li>Orange</li>
            <li>Mango</li>
            <li>Guava</li>
        </ul>
        ```

        এমন সিচুয়েশনে আমাদেরকে একটাই ইভেন্ট হেন্ডেলার বানাতে হবে যা দিয়ে সকল কম্পোনেন্টকে কনট্রোল করা যাবে এবং যদি আইটেম আরও বাড়ে তাতেও আমাদের ইভেন্ট হেন্ডেলার ঠিক ঠাক ভাবে কাজ করবে।

        এক্ষেত্রে আমরা list of items এর উপর ইভেন্ট হেন্ডেলার না নিয়ে তাদের প্যারেন্ট ইলিমেন্ট এর উপর ইভেন্ট হেন্ডেলার নিবো,তাহলে সকল লিস্ট আইটেম আমার ইভেন্ট হেন্ডেলার এর আন্ডারে চলে আসবে।

        `element.matches("something")` মাধ্যমে আমরা ইলিমেন্ট চেক করে চাইলে কন্ডিশনালি ইভেন্ট হেন্ডেলার ব্যাবহার করতে পারি ।

        **Event Propagation: Bubbling and Capturing**

        Propagation মানে হলো চলাচল করা বা ছড়িয়ে যাওয়া । জাভাস্ক্রিপ্টে event Propagation মানে হলো জাভাস্ক্রিপ্টে যে ইভেন্টগুলো আছে তা কোন ORDER এ চলাচল করবে ।

        ```jsx
        <div
            onClick={() => {
                alert("clicked on Parent Div");
            }}
            className='ParentDiv'>
            <div className='childComponent'>
                <div className='oneMoreDeepChild'>
                    <button
                        onClick={() => {
                            alert("clicked on Button");
                        }}>
                        Click Me
                    </button>
                </div>
            </div>
        </div>
        ```

        উপরের কম্পোনেন্টটিতে দেখা যাচ্ছে যে,একটা নেস্টেড কম্পোনেন্ট আছে,যার প্যারেন্ট `div` এ একটা `eventHandler` এ একটা এলার্ট দেয়া আছে এবং সেই সাথে একবারে শেষের চাইল্ড কম্পোনেন্ট `button` এ একটা `eventHandler` দেয়া আছে। এখন কথা হলো যদি আমরা `button` এ ক্লিক করি তাহলে প্যারেন্ট কম্পোনেন্ট এও তো ক্লিক পরে যাবে । এমতবস্থায় আমদের কোন ইভেন্ট হেন্ডেলারটি আগে রান হবে ?

        by Default দুটো ইভেন্ট হেন্ডেলার ই রান হবে,তবে সবার আগে বাটন এর ইভেন্ট হেন্ডেলার আগে রান হবে তারপর প্যারেন্ট কম্পোনেন্ট এর ইভেন্ট হেন্ডেলার রান হবে । এইযে একটা কম্পনেন্ট এ ক্লিক করলে অপর কম্পোনেন্টটাও ট্রিগার হয়ে যাচ্ছে এটাকে বলা হয় `Event Propagation`

        **Event Bubling**

        by default ইভেন্ট হেন্ডেলার ভিতর থেকে কল হয়ে বাহিরের দিকে যায়,উপরের এক্সাম্পল অনুযায়ী প্রথমে `button` এর ইভেন্ট হেন্ডেলার রান হবে তারপর প্যারেন্ট এর ইভেন্ট হেন্ডেলার রান হবে । এইযে ইভেন্টগুলো ভিতর থেকে কল হয়ে বাহিরের দিকে যাচ্ছে, এটাকে bubble এর সাথে তুলনা করা হয়েছে,আর এজন্য এটাকে বলা হয় `event Bubbling`

        **Event Trickling / Event Capturing**

        যেহেতু by default ইভেন্ট ভিতরের দিক থেকে কল হয়ে বাহিরের দিকে যায় ,এই বিহেভিয়ার চেঞ্জ করার জন্য মূলত ইভেন্ট কেপচারিং করা হয় , এজন্য আমদের ইভেন্ট হেন্ডেলারের third parameter এ capture:true দিয়ে দিলেই হয়ে যাবে। এটাকে বলা হয় `event capturing / event trickling`

        ```javascript
        element.addEventListener(
            "click",
            function () {
                //write some logic here
            },
            { capture: true }
        );
        ```

        **e.target**

        আমরা যখন কোন element এর উপর ক্লিক করি বা pointer করি তখন targeted element টা হলো `e.target`

        **e.current.target**

        কোন একটা pointer এ যদি multiple element target হয় তখন ১ম যেই element target হয়েছে সেটা হলো `e.current.target`

        **Event Propagation in React**

        `javascript` এর সকল ইভেন্ট রিয়াক্ট এ propagation হয় তবে শুধুমাত্র `onScroll` event এ রিয়াক্ট propagate করেনা ।

        **Stop Propagation in React**

        ```javascript
        e.stopPropagation(); // এভাবে আমরা রিয়াক্টে প্রপাগেশন স্টপ করতে পারি ।
        ```

    -   #### Understanding States - React Component's Memory - useState

        **What is State**

        স্টেট বলতে বুঝায় অবস্থা । কোন কিছুর অবস্থা বুঝাতে `state` শব্দটা ব্যাবহার করা হয়। রিয়াক্টে কোন কম্পোনেন্টের কোন অবস্থা বুঝাতে `state` ব্যবাহার করা হয়। রিয়াক্টে আমরা যখন কোন `state` ডিফাইন করি তখন এর ভিতরে তিনটা পার্ট থাকে ,

            1. state Name (It holds the initial value of state)
            2. setter function (It hepls to change the states values in different conditions)
            3. initial value (It remember the initial value of the state)

        ```javascript
        let initialState;
        const [count, setCount] = useState((initialState = 0));
        ```

        উপরের বলা তিনটা পার্টে বলা হয়েছে যে, রিয়াক্টে `state` এর একটা initial state থাকে, এই ইনিশিয়াল স্টেট টাকে রিয়াক্ট তার প্রতিটা রেন্ডারে মনে রাখে।

        `State` কে রিয়াক্ট কম্পোনেন্ট এর মেমরি বলা হয়ে থাকে,কেননা এর মেমরিতে একটা ইনিশিয়াল ডাটা সেভ থাকে যা রিয়াক্ট মনে রাখতে পারে তার প্রতিটা রেন্ডারে ।

        `State` এর একটা নেম ভেরিয়েবল থাকে যা তার ইনিশিয়াল ভ্যালুটা ধারন করে থাকে। আমরা যদি স্টেট এর ভ্যালু এক্সেস করতে চাই,তাহলে সেই নেম ভ্যারিয়েবল দিয়ে সেই ভ্যালু এক্সেস করতে পারি ।

        `State` এর একটা `setter function` থাকে যা দিয়ে আমরা চাইলে ইউজারের বিভিন্ন ইন্টারেকশন বা অন্যান্য বিভিন্ন কন্ডিশনে স্টেট এর ভ্যালু চেঞ্জ করে নতুন ভ্যালু সেট করতে পারি ।

        **Why we need to use State**

        আমরা যদি ইউজারের কোন ইন্টারেকশনের কারনে UI তে কোন পরিবর্তন করতে চাই এবং আমরা সেটা ম্যানুয়ালি ডমে আপডেট না করে শুধু একটা ভ্যালু চেঞ্জ করে দিয়েও করে ফেলতে চাই,তাহলে আমাদের `state` নিতে হবে ।

        আসলে রিয়াক্টিভ মানেই এটা । এই কারণেই রিয়াক্টের জন্ম । সাধারণত আমরা যখন ইউজারের কোন ইন্টারেকশনের কারনে UI এর কোন চেঞ্জ DOM এ দেখাতে চাই,তাহলে আমদের সেই DOM ELEMENT টাকে ধরে ম্যানুয়ালি চেঞ্জ করে আবার DOM আপডেট করতে হয় । কিন্তু রিয়াক্টে আমরা শুধুমাত্র setter function এর মাধ্যমে state এর ভ্যালু চেঞ্জ করে দেই,তখন রিয়াক্ট অটোমেটিক রি-রেন্ডার নিবে এবং উপডেটেড ভ্যালুটা UI তে দেখিয়ে দিবে ।

        **Hooks in React**

        React এ `useState`v হুক সহ আরও বেশ কিছু হুক রয়েছে, যেসকল ফাংশনের আগে `use` ব্যাবহার করা হয়েছে সেগুলোই রিয়াক্টের হুক হিসেবে পরিচিত। হুকগুলো হলো রিয়াক্টের স্পেশাল ফাংশন যা রিয়াক্টের রেন্ডারিং এর সময় ব্যাবহার করা হয়। এতে করে রিয়াক্টের রেন্ডারিং প্রসেসের মদ্ধে কিছু এক্সট্রা ফিচার এড করা যায়।

        **Where to define Hooks?**

        React এর হুকগুলো সবসময় কম্পোনেন্টে এর TOP LEVEL বা সবার উপরে ব্যাবহার করতে হয় । এগুলো কখনোই রিটার্নের ভিতরে বা কম্পোনেন্টের বাহিরে রাখা যাবেনা ।

        **Initial value Types of useState**

        `useState` হুক এর ইনিশিয়াল ভ্যালু হিসেবে আমরা যেকোন ধরনের ডাটা নিতে পারি যেমন ঃ `Array`,`object`,`number`,`string`,`boolean`

        **How Many State can be taken in One Component**

        একটা কম্পোনেন্ট এর ভিতরে আমরা আমাদের যতগুলো প্রয়োজন ততগুলো স্টেট নিতে পারি ।

        **State is Isoloted and Privet**

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

নিচের স্টেপ গুলোর মাধ্যমে আমরা রিডাক্স টুলকিট ব্যাবহার করতে পারি ।

`- Step : 1 :`

**Create A Slice**

```javascript
import { createSlice } from "@reduxjs/toolkit";
const someThingSlice = createSlice();
```

**Export Reducer from Slice**

```javascript
import { createSlice } from "@reduxjs/toolkit";
const someThingSlice = createSlice();

export default someThingSlice.reducer;
```

**Add Slice Name,initialState,reducers,extrareducers**

```javascript
import { createSlice } from "@reduxjs/toolkit";
const someThingSlice = createSlice({
    name: "someThingSlice",
    initalState: {
        data: [],
    },
    reducers: {},
    extrareducers: (builder) => {},
});

export default someThingSlice.reducer;
```

**Add reducer Actions**

```javascript
import { createSlice } from "@reduxjs/toolkit";
const someThingSlice = createSlice({
    name: "someThingSlice",
    initalState: {
        data: [],
    },
    reducers: {},
    extrareducers: (builder) => {},
});

export default someThingSlice.reducer;
```

**Handle Asyncronus call in ApiSlice file**

```javascript
import { createAsyncThunk } from "@reduxjs/toolkit";
import axios from "axios";
export const createNewPost = createAsyncThunk(
    "post/createNewPost",
    async (data) => {
        try {
            const response = await axios.post("http://localhost:7070/posts", {
                ...data,
                id: crypto.randomUUID(),
            });
            return response.data;
        } catch (err) {
            throw new Error(err);
        }
    }
);
```

**Add Extra Reducers when use Api for CRUD**

```javascript
import { createSlice } from "@reduxjs/toolkit";
import { createNewPost } from "./postApiSlice";

export const postSlice = createSlice({
    name: "post",
    initialState: {
        loading: false,
        error: null,
        message: null,
        postData: [],
    },
    reducers: {},
    extraReducers: (builder) => {
        builder
            .addCase(createNewPost.pending, (state, action) => {
                state.loading = true;
            })
            .addCase(createNewPost.fulfilled, (state, action) => {
                state.loading = false;
                state.postData = [...state.postData, action.payload];
            })
            .addCase(createNewPost.rejected, (state, action) => {
                state.loading = false;
                state.error = action.error.message;
            });
    },
});

export default postSlice.reducer;
```

-   `Step : 2 :`

**Create Store and Configure Store**

` create a file named 'store.js'`

```javascript
//store.js
import { configureStore } from "@reduxjs/toolkit";
import SomethingSliceReducer from "../SomethingSlice";
export const store = configureStore({
    reducer: {
        someThing: SomethingSliceReducer,
    },
});
```

-   `Step: 3 : `

**Pass store via Provider to App Component**

```javascript
//main.jsx
import { Provider } from "react-redux";
<Provider store={store}>
    <App />
</Provider>;
```

# useEffect Hook in React

**Syncronising With Effect**

-   ### কেন useEffect প্রয়োজন ?

    -   রিয়াক্টে আমাদের এমন কিছু টাস্ক সম্পন্ন করতে হয়,যা কোন ইউজারের ইন্টারেকশনের উপর ডিপেন্ড করেনা বরং সেগুলো আমাদের অটোমেটিক করতে হয় । এইসব কাজ গুলো হলো `side effect` । এগুলো কোন `event handler` এর উপর ডিপেন্ট করে কল হয়না ,বরং `Component` লোড হয়ে যাওয়ার পর আমাদের অটোমেটিক করে দিতে হয়। এই সমস্ত কাজ সম্পন্ন করার জন্য প্রয়োজন হয় `useEffect` এর ।

-   ### useEffect কিভাবে লিখতে হয় ?

    -   তিনটা স্টেপ এ `useEffect` লিখতে হয় ।

        -   **Declare an effect**
        -   **Specify the dependencies**
        -   **Add cleanup if needed**

    -   **Declare an effect**

        -   To declare an Effect in your component, import the useEffect Hook from React:

        ```
        import { useEffect } from 'react';
        ```

        Then, call it at the top level of your component and put some code inside your Effect:

        ```javascript
        useEffect(() => {
            //code will go here
        });
        ```

    -   **Specify the Effect dependencies**

        ডিফল্টভাবে যখন কম্পোনেন্ট মাউন্ট হয় তখনি useEffect কল হয় । তবে আমরা চাইলে `useEffect` ফাংশনের সেকেন্ড প্যারামিটার এ বলে দিতে পারি যে প্রথমবার লোড হওয়ার পর আর কখন কখন useEffect রান হবে। এজন্য useEffect এর সেকেন্ড প্যারামিটার এ আমাদেরকে `dependencies` গুলো বলে দিতে হয় ।

        `[] = লোড হওয়ার পর মাত্র একবার রান হবে পরে স্টেট চেঞ্জ হয়ে কম্পোনেন্ট রিরেন্ডার হলেও আর কখনোই রান হবেনা` ,

        `dependency= ডিপেন্ডেন্সি বলে দেয়া মানে হলো ডিপেন্ডেন্সি চেঞ্জ হলেই useEffect আবার রান হবে `

    -   **Add cleanup if needed** useEffect রান হওয়ার পর যখন কম্পোনেন্ট আনমাঊন্ট হবে তখন কিছু কিছু ক্ষেত্রে আমাদের কে useEffect cleanup করে দিতে হয় ,নাহলে effect যদি কম্পোনেন্ট Unmount হওয়ার পরও চলতে থাকে ,তাহলে সেকেন্ড টাইম যখন আবার কম্পোনেন্ট Mount হবে তখন তখনও যদি আগের effect রানিং থাকে এবং তার উপর আবারো effect কল হয় তাহলে এপ্লিকেশনে অনেক error and Bugs তৈরি হতে পারে।

### How to handle the Effect firing twice in development?

এজন্য প্রথমে আমাদের বুঝতে হবে যে,কেন `development` মুড এ আমাদের কম্পোনেন্ট দুইবার রান হয় ? এটা হয় মূলত `unpredictable bugs` খুঁজে বের করার জন্য। `React` ডেভেলপমেন্ট মুড এ প্রতিটা কম্পনেন্ট দুইবার করে রান করে,যাতে আমরা বুঝতে পারি যে আমাদের কম্পোনেন্টগুলো যদি দুইবার `mount` হয় তাহলে কোন `bug` তৈরি হয় নাকি । এজন্য রিয়াক্ট আমাদের প্রতিটা কম্পোনেন্ট প্রথমে Mount হবার পর সাথে সাথেই আবার `Unmonut` করে দিয়ে পুনরায় আবার `Mount` করে ।

### Mount,Unmount, Remount and Render, re-render

     ১। Mount = কম্পোনেন্ট টা ভিজুয়াল হওয়া । কোন কম্পোনেন্ট যখন আমাদের UI তে ভিজুয়াল হয় তখন সেটা হলো Mount.

     ২। Unmount = কোন কম্পোনেন্ট যখন আমাদের UI থেকে রিমুভ হয়ে যায় তখন তা হলো Unmount.

     ৩। Remount = কোন কম্পোনেন্ট UI থেকে রিমুভ হয়ে যাওয়ার পর তা আবারো UI তে ভিজুয়াল হউয়া ।

     ৪। Render = Render হলো react এর একটা কাজ ,যা রিয়াক্ট তার নিজের ভিতরেই করে থাকে। Render হলো মূলত কম্পোনেন্টটা লোড হওয়া ।

     ৫। Re-render = rerender ও রিইয়াক্ট তার নিজের ভিতরেই করে । এর মানে হলো কম্পোনেন্ট রিলোড দেয়া ।

### কিভাবে development মুড এ useEffect কাজ করছে ? কিভাবে দুই বার রান করছে ? কখন Mount/UnMount/ReMount হচ্ছে ?

-   প্রথমত কম্পোনেন্ট `Mount` হওয়ার সাথে সাথেই কম্পোনেন্ট আগে DOM এ render হয় । কপমোনেন্ট DOM এ রেন্ডার হওয়ার পর সাথেই সাথেই `useEffect` একবার রান হয়।

-   যেহেতু রিয়াক্ট এর ডেভেলপমেন্ট মুড এ প্রতিটা কম্পোনেন্ট দুইবার রান হয় তাই,প্রথমবার রান হওয়ার পর কম্পোনেন্ট unMount হয়ে যাবে এবং re-mount হয়ে যাবে ।

-   কম্পোনেন্ট যখন আবার re-mount হবে তখন useEffect আবার রান হবে । অর্থাৎ development mood এ প্রথমবারে কম্পোনেন্ট দুইবার Mount `(Mount -> UnMount -> Re-Mount)` হওয়ার কারনে `useEffect` ও দুইবার রান হবে ।

-   যদি useEffect এর ডিপেন্ডেন্সি বলে দেয়া থাকে তাহলে প্রথমবার useEffect রান হওয়ার পর একমাত্র যখন dependency চেঞ্জ হবে তখন আবার পুনরায় রান হবে । পুনরায় রান হওয়ার সময় যদি useEffect এ cleanup function থাকে,তাহলে প্রতিবার নতুন করে রান হওয়ার আগে আগের রান হওয়া effect টা clear করে দিবে।

    যদি dependency তে একটা [] থাকে তাহলে শুধু কম্পোনেন্ট Mount হওয়ার পর একবার রান হবে পরে আর কখনোই রান হবেনা ।

    যদি dependency না দেয়া থাকে তাহলে প্রতিবার কম্পোনেন্ট re-render হলেই useEffect রান হবে ।

**যদি cleanup function থাকে,তাহলে একমাত্র যখন কম্পোনেন্ট unMount হবে তখনি cleanup function রান হবে। কম্পোনেন্ট unMount না হলে কখনই cleanup function কল হবেনা**


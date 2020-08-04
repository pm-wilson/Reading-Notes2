# Reading Notes

## Foundations 2

### Due 8/3/20

- MDN (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals):

1. Template Literals are strings with embedded expressions. To use this, the backticks are used instead of the single or double quotes on a string.
2. The code to run is then in a \${}. By default expresions will concatenate into the text. Any new line characters will become part of the string.
3. This makes the code easier to read by developers.

- GoogleDeveloper (https://developers.google.com/web/updates/2015/01/ES6-Template-Strings):

1. Template strings are a way to define strings better. Rather than changing how existing strings work, template strings give us a different way.
2. Any valid JavaScript can be added into the strings, including functions. If you need backticks in your string, they can be escaped with the back slash.

- CSS Tricks (https://css-tricks.com/template-literals/):

1. Multiline strings are easy because the return is added as part of the string. This makes it very tidy to return HTML code broken down line by line.

- MDN forEach (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach):

1. Array.forEach() will execute a provided function (inside the parenthesis) once for each array element. It moves in ascending order and ignores any deleted indexes.
2. A this value can be given to the array.
3. Anything appended to the array during the call will be ignored. Later elements will be skipped if something shifts the array during the call.
4. It always returns undefined and does not mutate the array itself, but the function can. The forEach will not stop and there isn't a way to break out easily, so if this behavior is needed, use a different method.
5. Every(), some(), find(), findIndex() test the array elements and can be used to determine if the next iteration is required.
6. forEach will not wait for promises.
7. console.table() can be used to print a formatted version of an array.
8. Array.protype.flat() is a good way to flatten an array.

- vs forEach:

1. forEach() is a simpler way to loop through an array. The index value can also be given to refer back to. ForEach() only works on arrays, so it only helps for these situations. When you can use a forEach() it looks cleaner than a for loop.

### Due 8/4/20

- Part 1 (https://medium.com/backticks-tildes/visually-breaking-down-ui-components-using-atomic-design-part-1-476e1ddd73ca):

1. Atomic Design Methodology is building larger parts of a web site from smaller pieces and working your way up until you have your site. Molecules can be built so when new options are added, there might be something easily modified instead of re-built. This keeps the file structure modular.
2. To do this, start big with the skeleton and work your way down to smaller pieces. Organisms are the main sections, which are made of molecules (these might be repeated), which are made up of Atoms (single HTML elements).

- Part 2 (https://medium.com/backticks-tildes/visually-breaking-down-ui-components-using-atomic-design-and-building-with-react-part-2-20eb8aabab4b):

1. To make more complex pages, organize the code in folders depending on the Atomic level.
2. Start small and work your way up (as opposed to the opposite when breaking the design down visually)
3. Props can be utilized to make molecules more customizable.

- More Examples (https://theiconic.tech/the-art-of-transforming-ui-features-into-components-e86de5560fd7):

1. Building sites using Atomic Design has its own issues. Knowing what is already built can be difficult and having a developer add new code can interfere with what is already built.
2. Living Style Guides and Functional Pattern Libraries can be difficult to maintain.

- Thinking in React (https://reactjs.org/docs/thinking-in-react.html):

1. To break down the components, start with the design and draw boxes around everything. Every component should handle one thing, if it gets too complicated, it might need to be broken into more components.

- UI Components by Design (https://www.thoughtworks.com/insights/blog/ui-components-design):

1. Designers and developers think about different aspects and by using a common language can help eliminate confusion. Foundation components are targeted in scope and ensure a consistent product. Application components are specific to an application being built.
2. By designing smaller components and using them to build larger ones, designers and developers can stay on the same page as a site grows. With this, developers can focus on building complex logic rather than user interface details.

- What are JavaScript Callbacks? (https://www.sitepoint.com/callbacks-javascript/):

1. A callback is a function to be executed after another function. One useful purpose is to make sure a function has access to specific information before executing (like with API calls).

- JavaScript Callback Functions (https://www.dashingd3js.com/lessons/javascript-callback-functions):

1. Functions can be ran synchronous or asynchronous.
2. You can pass as many callbacks into a function as you want.

- First Class Functions (https://developer.mozilla.org/en-US/docs/Glossary/First-class_Function):

1. First Class Functions are functions that are treated as any other variable.

- MDN Callback Function (https://developer.mozilla.org/en-US/docs/Glossary/Callback_function):

1. Synchronous functions are used to return immediately, Asynchronous functions let other code run while it waits for more infomration.

- JavaScript Classes (https://javascript.info/class):

1. A class is a template for building objects.
2. A function created by Class gets checked for in a variety of places and must be called with new.
3. They are non-enumerable.
4. They can be made dynamically.
5. They may include get/set.

- An intro to object-oriented programming (https://www.freecodecamp.org/news/an-intro-to-object-oriented-programming-in-javascript-objects-prototypes-and-classes-5d135e7361b1/):

1. A class is a set of properties that particular objects share.
2. Class names begin with a capital letter and need the new operator which creates another copy per the template.

- Intro (https://javascript.info/object-methods):

1. The value of this is the object before the dot, the one used to call the method.
2. The rule is simple: if obj.f() is called, then this is obj during the call of f.
3. Arrow functions don't have their own this

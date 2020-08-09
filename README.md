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

### Due 8/5/20

- Responsive Web Design (https://learn.shayhowe.com/advanced-html-css/responsive-web-design/):

1. RWD is building websites suitable to all users
2. Rather than building separate sites for mobile, building a site that can adapt to mobile is a better idea.
3. CSS can adapt to screen size with vw, vh, vmin and vmax
4. target / context = result
5. Percentage and em can keep the page more flexible.
6. Media querys @media can tell css to use specific styles for specific screen sizes, orientations, ratios, resolution, and others.
7. Mobile first suggests building sites for mobile, and changing the styles if the screen is bigger to speed up mobile browsing.

- CSS Tricks Floats (https://css-tricks.com/all-about-floats/):

1. Float is a CSS position
2. A picture can float left of a text or right and the text will float around it. If text wrap is ignored the text continues over the picture.
3. Floated elements remain a part of the flow of the page, unlike absolutley positioned elements.
4. Clear will move the element down past the float, and takes left, right, both, none, inherit.
5. A parent element with only floats will collapse. To fix strange layout issues clear the float after the floated elements in the container, but before the close of the container.
6. Other method for clearing floats is the Empty Div, Overflow, clear:both.
7. Pushdowns can be fixed if the item inside the float is bigger than the container, overflow:hidden can fix this. Display: inline can fix a double margin in IE6. 3px Jog on text can be fixed by setting a width or height on the text. IE7 needs bottom padding instead of bottom margin.

-Grids (https://css-tricks.com/dont-overthink-it-grids/):

1. A block level element is as wide as its parent.
2. Start by setting the columns by their width and naming them well.
3. The parent will collapse so will need to be set to this: .grid:after{content:""; display:table; clear:both;}
4. Use box sizing: border-box for gutters
5. Then apply fixed padding to the right side of all but the last column.

- CSS Floats (https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/);

1. Floats create alternate flows, left and right. This allows the normal flow of elements to fill in the spaces around the floats.
2. Clear: both will block everything else so it doesnt get by.

- SMACSS Official Documentation (http://smacss.com/);

1. Base Rules are added to elements to define the default styling of the element. Resets should be used to strip out the defaults.
2. In the layout styles try to stick to classes, id styling can get complicated due to increasing specifictiy.
3. Element selectors can be used with child or descendent selectors.
4. State styles augment and override all other styles.
5. Themes and Typography styles should be grouped.
6. State changes are either class names, pseudo-class, media query.
7. Be careful when heavily relying on a defined HTML structure and if the HTML depth is too deep.
8. To speed things up use child selectors, avoid tag selectors for common elements, use class names as the right-most selector.
9. Prototype goals are to show states, review localization, isolate dependencies.
10. A preprocessor can let you use special syntax for css. They have useful features like variables, operations, mixins, nesting, functions, interpolation, file importing, extending.
11. Elements not used very often should still avoid being styled, they might be used in the future again.
12. Icon pictures can use sprites to reposition the background and show different pictures to minimize resources.
13. Inheritance can get complicated very quickly
14. To apply the principals use naming conventions that clarify purpose, ensure the CSS only affects the element it is supposed to, and reduce the depth of applicability
15. Avoid content specific context and name things flexibly.

### Due 8/6/20

- MDN URL Search Params.toString() (https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams/toString):

1. The URLSearchParams toString() method returns a query string suitable for use in a URL.

- URLSearchParams.toString() (https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams/toString):

1. same as above document.

- Built-in Loctaion Object (https://developer.mozilla.org/en-US/docs/Web/API/Location):

1. Location represents the URL of the object it is linked to. This works with the window and document.

- Hash change event (https://developer.mozilla.org/en-US/docs/Web/API/Window/hashchange_event):

1. The hashchange event happens when the fragment identifier of the URL has changed (the part that begins and ends with #)

- RegExr (https://regexr.com/):

1. An interactive app to help figure out how to reference text.

- Regex Tutorial (https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285):

1. Shows a handy guide to referencing text.
2. Helpful for data validation, scraping, wrangling, string parsing, replacement, syntax highlighting.

- Regex 101 (https://regex101.com/):

1. An interactive app to find ways to reference expressions.

- On Callbacks (https://flaviocopes.com/javascript-callbacks/):

1. Computers can typically only do one thing at once and interrupt other processes often and quickly to make it seem like multiple things happen at once.
2. JavaScript only does one thing at a time by default, but the browser provides APIs that can handle doing multiple things at a time.
3. The first callback in any callback is the error, which will be null as long as there is no error.
4. This callback nesting can complicate code and alternitaves include Promises and Async/Await.

- MDN on Asynchronous (https://flaviocopes.com/javascript-promises/):

1. A promise is considered a value that will eventually become available.
2. Promises start out in a pending state, which will eventually become a resolved or rejected state.
3. In JavaScript Battery, Fetch and Service Workers use promises.
4. Promises can be returned to other promises creating a chain.
5. If anything in the chain of promises fails and raises an error or gets rejected the control goes to the nearest catch() down the chain.
6. Promise.All() lets you define a list of promises and invoke something when they are all resolved.
7. Promise.Race() will run something when the first of the listed promises is resolved.

- Intro (https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous):

1. It can be difficult working asynchronously because you dont know how long it will take to get the data.
2. Async callbacks will excecute code in the background and once done it will call the callback function.
3. Promises are the new style. It will run the then() blocks when the data comes back and run the catch() if there is an issue.
4. Promises are made for asynchronous opearations and can handle more complex data calls easier. They are always called in the strict order they are placed. Error handling is much better. They avoid inversion of control when dealing with a third party library.

- Promises (https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Introducing):

1. A promise is a returned object to which you attach callbacks, instead of passing callbacks into a function.

- MDN Using PRomises (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises):

1. Promises handle things better when multiple things need to happen at once in a specific order.
2. Promises guarantee callbacks will never be called before the completion of the current run of the JavaScript event loop, callbacks added with then() will be called even after the success or failure of the operation, multiple callbacks can be added by calling then() on each and they will be invoked in order.
3. It is possible to chain after a failure.
4. Simple promise chains are best kept flat without nesting.
5. Mistakes to avoid include not returning something which breaks the chain, nesting uncecessarily can lead to uncaught errors, forgetting to terminate chains with catch() lead to uncaught promise rejections.
6. Best to either return or terminate promise chains, and return a new promise immediately to flaten things out.

- Video on Promises and Fetch (https://www.youtube.com/watch?v=IHjzyhjKxtc):

1. Fetch gets data from APIs.
2. fetch('url').then(function(response) {
   console.log or return(response.JSON())
   }).then(function(response) {
   console.log or return(response)
   }).catch(function(error) {
   console.log(error)
   })

- Promises in 20 Minutes (https://medium.com/quick-code/javascript-promises-in-twenty-minutes-3aac5b65b887):

1. Promises are easier to debugg than the nesting pyramid of doom

- Google Developer on Promises (https://web.dev/promises/):

1. Async wont do a good job of catching errors that happened before the last one.
2. A promise can be fulfilled, rejected, pending, settled
3. JavaScript promises are compatable with Q promises.
4. Promises offer the best in parallelism and sequencing.

- MDN using fetch (https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch):

1. Fetch makes a url request and returns a promise. The promise resolves with a response object. We call a response method to read the body of the response.
2. Along with getting data, Fetch can also post and do other actions with data.

- Fetching data (https://itnext.io/that-data-looks-so-fetching-on-you-understanding-the-js-fetch-api-880eae0c8d25):

1. The fetch promise wont reject on HTTP error status, just on network failure. Fetch can receive cross site cookies. Fetch can send cookies if you set the credentials init option.
2. The Headers() constructor lets you create your own headers. This can be good to check the type of data you are receiving.

### Due 8/7/20

- Heroku: Getting Started with Node (https://devcenter.heroku.com/articles/getting-started-with-nodejs):

1. Instructions on how to setup and get started with Heroku, installing a starter app, and add ons.
2. Unable to deploy the app, the page says to run 'heroku create' in the console in the newly created cloned repo, but I get a heroku: command not found.

- Deploying a Simple Blog to Heroku (https://howtonode.org/deploy-blog-to-heroku):

1. I will get this going once I get through the installation steps.

- Problem Solving Skills (https://ryanstutorials.net/problem-solving-skills/):

1. Being a good problem solver includes being open minded, inquisitive, asking the right questions. Slowing down, not beign lazy and not panicing are also important.
2. The process includes assessing the situation, creating a hypothesis, and testing it.
3. Understanding the relationship between things, and breaking the problem down into smaller pieces helps.
4. When thinking about something complex, think of 3 solutions before getting started. Share them with an uninterested observer.

- Improve Critical Thinking (https://hbr.org/2019/05/3-simple-habits-to-improve-your-critical-thinking):

1. Good critical thinking includes questioning assumptions, reasoning through logic, and diversifying thought.

- Asking Great Questions (https://hbr.org/2018/05/the-surprising-power-of-questions):

1. It is important to be a good listener when asking questions.
2. Research shows conversations are for learning and liking.
3. Asking a lot of questions does both.
4. Keep follow up questions.
5. Know when to use openended questions.
6. Ask tough questions first to open people up.
7. use the right tone and pay attention to group dynamics.

### Due 8/10/20

- Node Express (https://www.sitepoint.com/an-introduction-to-node-js/):

1. Node is a JavaScript runtime built on Chrome's V8 JavaScript engine.

2. Node is an event-based, non blocking, asynchronous I/O runtime that uses Google's V8 JavaScript engine and libuv library.

3. Node programs are like JavaScript in browsers, but is a run time on a computer.

4. Rather than installing node binaries for your system, you can install a version manager that can use different versions for different applications.

5. Node.js lets us run JavaScript on a server. It handles requests asynchronously, but unhandled errors can cause big problems.

6. Node is particulary suited to build apps that need real time interaction like chats.

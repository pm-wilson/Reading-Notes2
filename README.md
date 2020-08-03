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

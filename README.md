# react-style-guide
A style guide for managing sane react components.

From using React for a month my initial thoughts.

# Components
  1. Don't get fancy with manipulating child DOM elements. If you see yourself mapping over them, create a Component instead!
  2. Once you see duplicated functionality in your components, use a Mixin.
  3. Don't change state in a child component without letting the parent component know.
  4. Deeply nested component.. are really hard and can be confusing at times.
  5. Class methods, should do one thing. (Single Responsibility Principle)
  
# Commenting
  1. Write a comment at the top of the file of who the parent is.
  2. 
  
# Mixins
  1. Use more mixins.
  2. Can you use mixin for duplicated renders?
  3. I like to prefix mixin methods with ```_mxn_```, so in my components I write ```this._mxn_functionName``` and I know it's from a mixin.
  4. 
  
# CSS in your components.... hmmmm
  I still think about this a lot but it's very nice and useful when you're creating dynamic css styles for your components.
  1. abstract your css into a class method. ~~~ cssStyles: function(){...} ~~~
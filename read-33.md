# *Conditional Rendering*

> *Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.*


# *Lists and Keys*

> *Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:*


``` ruby
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
```

# *Forms*

> *HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:*

``` ruby 
<form>
  <label>
    Name:
    <input type="text" name="name" />
  </label>
  <input type="submit" value="Submit" />
</form>
```

# *Lifting State Up*

> *In this section, we will create a temperature calculator that calculates whether the water would boil at a given temperature.*

> *We will start with a component called BoilingVerdict. It accepts the celsius temperature as a prop, and prints whether it is enough to boil the water:*

``` ruby
function BoilingVerdict(props) {
  if (props.celsius >= 100) {
    return <p>The water would boil.</p>;
  }
  return <p>The water would not boil.</p>;
}
```

# *Composition vs Inheritance*

> *React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.*

> *In this section, we will consider a few problems where developers new to React often reach for inheritance, and show how we can solve them with composition.*


# *Containment*

> *Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.*

> *We recommend that such components use the special children prop to pass children elements directly into their output:*

``` ruby
function FancyBorder(props) {
  return (
    <div className={'FancyBorder FancyBorder-' + props.color}>
      {props.children}
    </div>
  );
}
```

# *Thinking in React*

> *React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.*

> *One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.*

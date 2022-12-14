- React events are named using camelCase, rather than lowercase and they start with `on` in the built in components
- As a convention we can add our own on props (props that start with `on`) for our custom components.
- When using React, you generally don’t need to call addEventListener to add listeners to a DOM element after it is created.
 Instead, just provide a listener when the element is initially rendered.
- We pass a function to the `on` prop as an event handler.
- We want to keep the JSX code inside the return block clean and clear without too much logic inside. So we aim to separate
code into smaller components and separate logic into functions declared before the return block.
- We point to the function of the event handler in the `on` prop, means we write the name of the function without the
parenthesis ()

Why? Because we don't want to run the function when the JSX is evaluated/parsed which is too early to run, instead we want
the function to run only when the event happens ex: only onClick

- As a convention end your function name with `Handler` to know it's attached to event listener ex: `clickHandler`


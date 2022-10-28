- React Refs allow you to reference a DOM HTML element from within a parent component to give you a direct access 
to modify it without state update.
- React Refs should only be used when they are necessary 
- Using Refs is imperative because we are directly telling React that we want the picture to be painted
in an exact way
- useRef hook has been implemented as a solution to use React Refs within functional components
- 3 steps are required to do that:
    - Declaration step:
      - `const submitBtnRef = useRef(initialValue)`
      - useRef returns a mutable ref object whose .current property is initialized to the passed argument (initialValue)
    - Attach it to an element
      - `<button className='new-expense__actions' type='submit' ref={submitBtnRef}>`
      - React will set its .current property to the corresponding DOM node whenever that node changes.
    - Access and modify:
      - `submitBtnRef.current.doSomething()`
      - `.current` property is mutable means it can change at anytime.
      - Mutating the `.current` property doesn’t cause a component re-render

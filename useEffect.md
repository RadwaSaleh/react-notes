![image info](./resources/useEffect.png)
- You should add "everything" you use in the effect function as a dependency - i.e. all state variables and functions you use in there.
- You must add all "things" you use in your effect function if those "things" could change because your component (or some parent component) re-rendered.
- Exceptions:
    - state updating functions
    - built-in APIs or functions
    - variables (not some state or a prop) or functions you might've defined OUTSIDE your components

- Inline Styling: more and duplicate code
- Dynamic Styling: 
- Conditional Inline and Dynamic Styling:
    - CSS file with class names that is imported in the js file
    - Any other components can import this file and use same class names
    - Globally Scoped 
    
- Two examples of scoped CSS 
    - Styled Components: 
      - a package that helps you build a component that has a certain style 
      - This style affects only the attached component.
      - styled-components generate unique class names for your styles. You never have to worry about duplication.
      - Painless maintenance because you never have to go across different files to find the styling affecting your component
      - Styled Components can be nested
      - You can pass props to the Styled Components
      - You can apply styles globally to an application using Global Styles feature:
          - you apply styles globally to an application, for example to:
              - Set a font-family for all your typography
              - Set the background color on every page
              - Override browser default styling

    - CSS Modules: 
      - "CSS files in which all class names and animation names are scoped locally by default".
      - File name convention `Button.module.css`

# src/scss folder architecture

## scss/

This folder holds all of the designated folders that hold the SCSS files.

### _main.scss

This file is the the main file that all the other files are imported into. The files are listed in order of how you want the styling applied.

### abstracts/

This folder concerns itself with the variables and styles that are used across the entire application.

#### _functions.scss

This allows you to define complex operations on SassScript values that you can re-use thorughout your stylesheet.

They make it easy to abstract out common formulas and behaviors in a readable way.

Functions are defined using the @function at-rule, which is written @function <name>(<arguments...>) {...}.

#### _variables.scss

You assign a value to a name that begins with $, and then you can refer to that name instead of the value itself. 

If there is every a need to change the design system, you only need to change it in your variables file instead of hunting to try to find every place you declared a color.

#### _mixins.scss

This allows you to define styles that can be re-used throughout your stylesheet. 

They make it easy to avoidm using non-semantic classes like: float-left, and to distribute collections of styles in libraries.

### base/

This folder is where a version of a CSS Reset would be and where you would define anything that concerns the font of your webpage.

#### _typography.scss

This file is all about style, proportiions, and spacing.

#### _reset.scss

This file is used to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on.

### components/

This folder will have structural specific rules for buttons, carousels and other such elements. Each componet should have its own file.

#### _header.scss

This file will control specific details about what the webpage header will look like.

### pages/

This folder looks at each individual page's style

#### _home.scss

This file looks at the variables, typography, and header files.

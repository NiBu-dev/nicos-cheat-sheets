# Lecture 1

**Angular** - *is a javascript framework which allows to create reactive single page applications*.

*Note* - Javascript changes the DOM, the HTML.

# Lecture 9

**TypeScript** - *is superset of javascript* -> is compiled to javascript (here come the CLI usage) ->where is run from the browser

**TypeScript** -> Compilation -> **JavaScript** -> **Browser**

# Lecture 10 
## Bootstrap

To install bootstratp in the project:

    npm install --save bootstrap@3

Add the bootstratp to the project in the angular.json file, css array field:

    "node_modules/bootstrap/dist/css/bootstrap.min.css"

# Lecture 18
## Create an app component using CLI
Create a component called servers

    ng generate component servers
    
or

    ng g c servers

## Lecture 22
## Data binding

Databinding = Communication between the logic and view (functionality <> html template)

**Types of communication** :
* Output data (from logic ->  to view)
    * String interpolation ({{ data }})
    * Property binding ([property]="data")
* Input from user (event react)
    * Event binding ((event)="expression")
* Combination of both directions (inout and output)
    * Two way binding ([(ngModel)]="data")
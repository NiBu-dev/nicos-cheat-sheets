# Lecture 1

**Angular** - *is a javascript framework which allows to create reactive single page applications*.

*Note* - Javascript changes the DOM, the HTML.

# Lecture 9

**TypeScript** - *is superset of javascript* -> is compiled to javascript (here come the CLI usage) ->where is run from the browser

**TypeScript** -> Compilation -> **JavaScript** -> **Browser**

# Lecture 18
## Create an app component using CLI
Create a component called servers

    ng generate component servers
    
or

    ng g c servers

or

    ng g c servers --spec false

to skip the creation of the testing file

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

## Lecture 32
## Directives

Directives = instructions in the DOM (almost like a component without a template)

* Structural directives start with a star (*)

Unlike structural directives, attribute directives don't add or remove elements. They only change the element they were placed on.

## @Input and @Output

@Input - decorator used to send data from parent to child. The data is binded in the parent.html:

    [child_data]='parent_data'

and sent to the child.html, where it is taken as an input:

    @Input() child_data: string

@Output - decorator used to send data from child to parent. Usually used to pass events. The event is binded in the parent.html:

    (child_event)="parent_event_handler($event)"
 
 and the event is sent from child as 
 
     @Output() child_event = new EventEmitter(data: string)

## Directives

### Attribute directives

Looks like a normal HTML  attribute (possibly with databinding or event binding)

Only affect/change the element they are added to

### Structural directives

Looks like a normal HTML attribute but having a leading *

Affect a whole area in the DOM (elements get added/removed)

## Services

Ussualy services are use to share data with several components.

Services are hierachicall structured: i.e. the service provided in app.module.ts can be accessed within the all application. 
On the other hand, the services defined at the leaf components of the application can be accessed only by that component, even overiding the similar service instance inherited from parent component.

The services are provided by using the following definition within component:

   providers: [ Service_dummy ]

If using service within a service, the metadata has to be attached to the parent service, where the main service is used:

    @Injectable()

    export class Service_dummy {

    }

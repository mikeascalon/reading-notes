# Reading Notes

## Domain Modeling

1.Explain why we need domain modeling.

* Domain modeling allows developers, domain experts, and stakeholders to create a shared understanding of the problem space.

## HTML Table Basic

1.Why should tables not be used for page layouts?

* Layout tables reduce accessibility for visually impaired users

2.List and describe 3 different semantic HTML elements used in an HTML `<table>`.

* `<caption>` element is used to provide a title or a brief description for the entire table

* `<thead>` These elements group the rows of a table into different sections, providing semantic meaning and helping assistive technologies understand the table's structure.

* `<th>` element is used to define table header cells in the `<thead>` section or to provide semantic meaning to header cells within the main body of the table.

## Introducing Constructors

1.What is a constructor and what are some advantages to using it?

 a constructor is a special method or function that is automatically called when an object of a class is created or instantiated. 

2.How does the term this differ when used in an object literal versus when used in a constructor?

* Object Literal:
When this is used within an object literal (i.e., when defining an object using curly braces {}), it refers to the object itself, which is the object containing the property or method where this is used.

* Constructor Function:
When this is used within a constructor function, it refers to the instance of the object being created by the constructor

## Object Prototypes Using A Constructor

1.Explain prototypes and inheritance via an analogy from your previous work experience

* In your dental clinic, you create "prototypes" for each type of dental instrument. For example, you have a "ToothbrushPrototype" for all toothbrushes, a "ScalerPrototype" for all scalers, and a "MirrorPrototype" for all dental mirrors. These prototypes define common attributes and functions that instruments of the same type should share. For instance, they specify that all dental instruments should be sterilizable and have a handle for gripping.

* Inheritance in JavaScript can be likened to the relationship between the dental instrument prototypes and their instances. Just as actual dental instruments inherit attributes and functions from their prototype, JavaScript objects inherit properties and methods from their prototypes. This means that a toothbrush "inherits" the general properties and functions from the "ToothbrushPrototype."

### Resources

[HTML table basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

[JavaScript object basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

Chat GPT

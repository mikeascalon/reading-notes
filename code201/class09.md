# Reading Notes

## HTML Forms

1.Why are forms so important in web development?

* Forms enable user interaction, data collection, and communication.

2.When designing a form, what are some key things to keep in mind when it comes to user experience?

 important to remember that the bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.

3.List 5 form elements and explain their importance.

a.Text Input (Text Box) -fields allow users to enter short text, such as names, email addresses, and search queries.

b.Radio Button- present a list of mutually exclusive options, where users can select only one choice.

c.Checkboxes-allow users to make multiple selections from a list of options.

d.Dropdown Menus (Select)-  provide a space-efficient way to present a list of options, conserving screen real estate.

e. Text Area (Textarea)-sed for longer text input, such as comments, feedback, or essay-like responses.

## Introduction to Events

1.How would you describe events to a non-technical friend?

When somebody touch your skin . Event is your skin is telling you brain that something touch your skin .
2.When using the addEventListener() method, what 2 arguments will you need to provide?

* The first argument is the type of event you want to listen for. This is a string that specifies the type of event you're interested in, such as "click," "keydown," "submit," "mouseover," or any other valid event type.

* The second argument is a function that defines the action you want to take when the specified event occurs. This function is often referred to as an "event handler" or a "callback function." It is the code that will run in response to the event. This function will be executed when the specified event takes place.

3.Describe the event object. Why is the target within the event object useful?

* The event object is a built-in JavaScript object that contains information about an event that has occurred in the web browser. When an event is triggered, such as a click, mouseover, or keypress, the browser creates an event object and passes it as an argument to the event handler function you've registered using addEventListener()

4.What is the difference between event bubbling and event capturing?

* In the bad old days, when browsers were much less cross-compatible than now, Netscape only used event capturing, and Internet Explorer used only event bubbling. When the W3C decided to try to standardize the behavior and reach a consensus, they ended up with this system that included both, which is what modern browsers implement.

### Resources

[HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

[Introduction To Events.](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

ChatGPT

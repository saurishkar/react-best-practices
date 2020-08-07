## Form Best Practices

### 1. A form should have it's own component
<p>
Keeping a separate component for a form helps encapsulating internal form functions.
</p>

### 2. Do not render over-engineered form inputs
<p>
I had a login form in which i had rendered all <b>input(text, email or password)</b> elements dynamically using a single <b>renderField</b> function.
This looks compact but reduces the flexibility for each of the form inputs.

Better approach will be to render the JSX of the form element normally, so that in case atleast 1 of the elements need to have an attribute different from others,
it can be easily added without breaking all other form inputs.

Form inputs like radio buttons or checkboxes which share same attributes can be dynamically rendered.
</p>

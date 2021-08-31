# Read 4: React and Forms

### * React - Forms:
- **What is a ‘Controlled Component’?**

       A controlled component is a component that renders form elements and controls them by keeping the form data in the component's state.

- **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

       I think we should update the state after their response , because the state is going to be empty in the first place.

- **How do we target what the user is entering if we have an event handler on an input field?**

        By using HOOKS, you can create a variable for each input field, and listening on the onChange event you call the “set” function for that variable.


### * The Conditional (Ternary) Operator Explained:

- **Why would we use a ternary operator?**

      we can display the contents on the basis of one condition where everything depends on the condition true and false we can put the contents on the conditional basis.


** EX: **

      if(x===y){
      console.log(true);
        } else {
      console.log(false);
        }

  ** In Ternary Operator: **

            console.log((x===y) ? 'true' : 'false');
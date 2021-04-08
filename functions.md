# Functions

* [Create a function](functions.md#create-a-function)
* [Create a function with an output](functions.md#create-a-function-with-an-output)
* [Create a conditional function](functions.md#create-a-conditional-function)

## Create a function

![](.gitbook/assets/blocks-function-fig-1.png)

To create a function, you will need to specify if it has any inputs and give it a name

![](.gitbook/assets/blocks-function-fig-5.png)

One example of a function is below. This function will create and shuffle a list of items.

![](.gitbook/assets/screen-shot-2021-04-08-at-11.10.29-am.png)

After you have created your function, you can simply use it at any time using the function block you have named

![](.gitbook/assets/screen-shot-2021-04-08-at-11.11.45-am.png)

## Create a function with an output

You can also create a function that returns a specific output.

![](.gitbook/assets/doandreturn.png)

### Conditional Outputs

You can add multiple `return` blocks to your function. This allows you to return a different output based on some conditions.

For example, this function will take a rating out of 100, and return a description of the quality of the item being reviewed:

![](.gitbook/assets/qualfunc.png)

The function will break when the `return` block is fired. For example, in the above example, if the quality rating is 100, the function will return **Perfect** and then stop. It will not run the other tests, and won't return **Excellent**. **Good**, **Fine**, etc.


Exercise 1: Pad numbers

Lets practice how to use code from other developers in our applications. I wrote the following function this other day:

function padLeft(val, num, str) {
	return '00000'.replace(/0/g, str).slice(0, num - val.length) + val;
}

This function adds characters to a string so that it has at least a certain number of characters. For example. padLeft('foo', 5, '') returns " foo" and padLeft('5', 2, '0') returns "05". Pretty neat huh!?

You find this function brilliant and want to use it in your code. Follow the steps:

    Create a new empty folder, e.g. 1-pad-numbers inside your week1 homework folder
    Inside, create a file called padLeft.js, then copy the function padLeft in it.`
    Also create file called app.js.
    In this file use the padLeft function from padLeft.js to pad the numbers = [ "12", "846", "2", "1236" ] to exactly 4 spaces then print each padded number in the console.

Expected output (replace the underscore with spaces):

___12;
__846;
____2;
_1236;

Tips:

    use the exports keyword in padLeft.js
    use the require keyword in app.js
    use forEach to loop over the array in app.js
    use padLeft(number, 4 , " ") to pad a number to 4 characters


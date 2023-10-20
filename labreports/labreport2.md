# Lab Report 2

## Part 1

StringServer Code:

![Image](../labreport2-images/code.png)

Adding "Hello:"

![Image](../labreport2-images/add-message1.png)

Here, the `handleRequest` method is being called, as it is when any URL is created. The method will use the URL as the argument and, in this case, detect that the path of the URL contains `/add-message`. It will then store the message that is being added in a string array called `parameters`, which is then used to add the new word to the list. Two values change from this request: the `words` string containing the list of words, and the integer `num` which keeps track of how many words there are so it can display the numbered list correctly.

Adding "How are you:"

![Image](../labreport2-images/add-message2.png)


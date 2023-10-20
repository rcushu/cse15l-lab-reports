# Lab Report 2

## Part 1

**StringServer Code:**

![Image](../labreport2-images/code.png)

**Adding "Hello:"**

![Image](../labreport2-images/add-message1.png)

Here, the `handleRequest` method is being called, as it is when any URL is created. The method will use the URL as the argument and, in this case, detect that the path of the URL contains `/add-message`. It will then store the message that is being added in a string array called `parameters`, which is then used to add the new word to the list. Two values change from this request: the `words` string containing the list of words, and the integer `num` which keeps track of how many words there are so it can correctly display the numbered list. Finally, the method will return a string saying that your word has been added.

**Adding "How are you:"**

![Image](../labreport2-images/add-message2.png)

Mostly everything is the same in this case, with the exception of  `words` being updated with a different string and number, and the return message being different. This is functionally identical to the last example.

## Part 2

![Image](../labreport2-images/keys.png)

![Image](../labreport2-images/ssh-login.png)

# Lab Report 5

## 1.

![Image](../labreport5-images/labreport5-1.png)

## 2.

![Image](../labreport5-images/labreport5-2.png)

## 3.

![Image](../labreport5-images/labreport5-3.png)

![Image](../labreport5-images/labreport5-3-1.png)

After trying what the TA suggested, it is now clear that the issue with the code is present in the `while` loop responsible for merging `list1` into `result`

![Image](../labreport5-images/labreport5-3-2.png)

Looking at the `while` loop in question, it can be seen that the `while` loop runs while `index1` is greater than the size of `list1`. `index1` begins as `0` when the method is ran, and since `index1` will never be greater than the size of `list1`, this `while` loop is never executed and the contents from `list1` are never added to `result`.

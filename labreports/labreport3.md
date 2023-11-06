# Lab Report 3

## Part 1

### **List Examples `reverseInPlace` method:**

![Image](../labreport3-images/reverseInPlace.png)

### Failure Inducing Input:

JUnit Test:
```
@Test 
public void testReverseInPlace() {
    int[] input1 = { 3, 2, 1 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 1, 2, 3 }, input1);
}
```
Input: `{ 3, 2, 1 }`

Expected:   `{ 1, 2, 3 }`

Actual:     `{ 1, 2, 1 }`

### Non-Failure Inducing Input:

JUnit Test:
```
@Test 
public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
}
```

Input: `{ 3 }`

Expected:   `{ 3 }`

Actual:     `{ 3 }`

### Symptom:

Failure:

![Image](../labreport3-images/failure.png)

No failure:

![Image](../labreport3-images/noFailure.png)

### Bug:

Before:

```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
}
```

After:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int temp = arr[i];
      arr[i] = arr[arr.length - 1];
      arr[arr.length - i - 1] = temp;
    }
}
```

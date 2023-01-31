# Lab Report 2 - Servers and Bugs
## String Server
![image](https://user-images.githubusercontent.com/122576045/215695268-750807c7-6c37-4eda-93d1-45cd4fb28a27.png)

![image](https://user-images.githubusercontent.com/122576045/215695199-94a930b3-eefe-43ac-96e2-a8902931e21f.png)

***
## reverseInPlace() Bug
Failure Inducing Input:
```@Test
    public void testReverseInPlace2() {
   	 int[] input1 = {4,5,6};
   	 ArrayExamples.reverseInPlace(input1);
   	 assertArrayEquals(new int[]{6,5,4}, input1);
    }
```
Non-failing Input:
```@Test
    public void testReverseInPlace2() {
   	 int[] input1 = {5};
   	 ArrayExamples.reverseInPlace(input1);
   	 assertArrayEquals(new int[]{5}, input1);
    }
```
Respective Symptoms:

The bug in the code:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
```
The fix:
```
static void reverseInPlace(int[] arr) {
    int[] tempArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      tempArray[i] = arr[arr.length - i - 1];
    }
    arr = tempArray;
  } 
 ```
 In the original code, the array elements are not copied to another array, so then the for loop misinitializes some elements and does not properly reverse the elements, as traversal through the array allows elements that have already been placed in their properly reversed order to be placed again in a different, potentially incorrect index. The fixed code copies the array elements into a temporary array and iterates through both the temporary and parameter array, ensuring that traversal of the for loop will not duplicate elements in potentially incorrect indices in the original/parametr array. 
***
## Something I learned
The primary subject I learned about in the completion of these two lab activities was the existence of URIs: to be specific, I did not even know of the existence of URIs and thus learned significantly about them.

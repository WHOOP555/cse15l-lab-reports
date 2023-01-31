# Lab Report 2 - Servers and Bugs
## StringServer.java
The code:
```
import java.io.IOException;
import java.net.URI;
class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String data = "";
    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return data;
        } else if (url.getPath().equals("/add-message")) {
            String toConcat = url.getQuery().substring
            (2, url.getQuery().length()) + "\n";
            data = data + toConcat;
            return data;
        } 
        else {
            return "404 Not Found!";
        }
    }
}
public class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
![image](https://user-images.githubusercontent.com/122576045/215695268-750807c7-6c37-4eda-93d1-45cd4fb28a27.png)
1. In the above screenshot, first of all the handleRequest() method is called. Next, the getPath() method is called. After this, the equals() method is called. Then, the getQuery() method is called, followed by a call to .substring(), .getQuery(), and .length().
2. The argument for the handleRequest() method is the respective URI (/add-message?s=Hello), and there is no argument for the rest of the methods except .equals(), whose argument is the String "/add-message", and .substring(), whose argument is the int 2 and the int url.getQuery().length(), which is 7. 
3. After the passing of the method, the value of the field, data, is merely the String "Hello" + "\n", while the value prior to this was simply the empty String.
![image](https://user-images.githubusercontent.com/122576045/215695199-94a930b3-eefe-43ac-96e2-a8902931e21f.png)
1. In the above screenshot, first of all the handleRequest() method is called. Next, the getPath() method is called. After this, the equals() method is called. Then, the getQuery() method is called, followed by a call to .substring(), .getQuery(), and .length().
2. The argument for the handleRequest() method is the respective URI (/add-message?s=potatoes), and there is no argument for the rest of the methods except .equals(), whose argument is the String "/add-message", and .substring(), whose argument is the int 2 and the int url.getQuery().length(), which is 10. 
3. After the passing of the method, the value of the field, data, is merely the String "Hello" + "\n" + "potatoes" + "\n", while the value prior to this was just "Hello" + "\n".
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

# Lab Report Number 2: JayLynne Redeaux 
## __Part One:__
> 
> > Code: 
> > ![image](https://user-images.githubusercontent.com/130107248/234170525-1f2f9aad-c7ee-45dd-b54f-f662d336acc1.png)
![image](https://user-images.githubusercontent.com/130107248/236961437-2eb87267-22f0-4c17-9b71-62acc20b96ef.png)
>Methods called:
>* handleRequest(URI url) in the __Handler__ class
>>The relevant arguments to the handleRequest method in the Handler class are:
>* url
>>The relevant fields of the Handler class are:
>* output
>>Within the handleRequest method, the relevant values are:
>* url.getPath() -> /add-message
>* url.getQuery()
>* param[0] -> s 
>* param[1] - > hello
>* output -> changes to: "Hello\n"

![image](https://user-images.githubusercontent.com/130107248/236962877-df126c8f-ffbb-4526-93ed-20d03baa6d78.png)
The only changes we have are within the relevant values, questions 1 and 2 remain the same from the first screenshot. 
>>Within the handleRequest method, the relevant values are:
>* url.getPath() -> /add-message
>* url.getQuery() -> "s=Hello%20how%20are%20you"
>* param[0] -> "s" 
>* param[1] - > "Hello how are you"
>* output -> changes to: "Hello\nHello how are you\n"
>
__Part Two:__
>__Input that does induce failure:__ 
>
  >`@Test
  >public void testReversed() {
  >  int[] input1 = { };
  >  assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  >}`
> 
> __An input that does induce a failure:__
 
>`@Test
  public void testReversed2() {
    int[] input1 = { 10, 5, 0 };
    assertArrayEquals(new int[]{0,5,10 }, ArrayExamples.reversed(input1));
  }`
>
> __The Symptoms Of both Inputs:__
> ![image](https://user-images.githubusercontent.com/130107248/234173007-aaa68a2f-424d-4619-b3aa-89d30fcc72c3.png)

>__The code Before and After (The bug 🐞 )__:
>
>Before :   
 `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }`
 
>After :
 ` static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray; 
    `
> To fix the bug, we changed the assignment statement in the for loop to copy the value from the original array to the new array rather than overwriting it. We also changed what we returned, we returned the new array instead of the old array. 


>__Part 3:__
>In week 2's lab I learned a lot about starting servers and how to implement changes based on paths inputted. Specifically, I learned about the command `curl` that lets me acess URLs from the command line. Instead of opening a web browser everytime I can rtun the command in my terminal to load the URL. I found this helpful because switchiing between safari and VSCode was tedious. 

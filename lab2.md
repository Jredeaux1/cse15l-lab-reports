# Lab Report Number 2: JayLynne Redeaux 
## __Part One:__
> I am having a hard time with this and need to go to tutoring to get help with my outputs. I will be resubmitting this part. I didnt want to leave this empty so I will show my code so far that isnt running anymore. 
> > Code: 
> > ![image](https://user-images.githubusercontent.com/130107248/234170525-1f2f9aad-c7ee-45dd-b54f-f662d336acc1.png)

__Part Two:__
>__Failure inducing code:__ 
>
  >`@Test
  >public void testReversed() {
  >  int[] input1 = { };
  >  assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  >}`
> 
> __An input that doesn’t induce a failure:__
 
>`@Test
>public void testReversed() {
>int[] input1 = { };
>assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
>}`
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
    return newArray; `
> To fix the bug, we changed the assignment statement in the for loop to copy the value from the original array to the new array rather than overwriting it. We also changed what we returned, we returned the new array instead of the old array. 


>__Part 3:__
>In week 2's lab I learned a lot about starting servers and how to implement changes based on paths inputted. Specifically, I learned about the command `curl` that lets me acess URLs from the command line. Instead of opening a web browser everytime I can rtun the command in my terminal to load the URL. I found this helpful because switchiing between safari and VSCode was tedious. 

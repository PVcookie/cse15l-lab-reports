# Week 2 Lab Report - Servers and Bugs

## Part 1 - StringServer
**Code**

'

    import java.io.IOException;
    
    import java.net.URI;
    
    import java.util.ArrayList;

    class Handler implements URLHandler {
        ArrayList<String> msg = new ArrayList<String>();

      public String handleRequest(URI url) {
          if (url.getPath().equals("/")) {
              return String.format("Type a message!");
          } else {
              System.out.println("Path: " + url.getPath());
              if (url.getPath().contains("/add-message")) {
                  String[] parameters = url.getQuery().split("=");
                  if (parameters[0].equals("s")) {
                      String input = "";
                      for(int i = 1; i < parameters.length; i++){
                          input += parameters[i];
                      }
                      msg.add(input);
                  }
              }
          }
          return String.format(String.join("\n", msg));
      }
    }

    class StringServer {
      public static void main(String[] args) throws IOException {
          if(args.length == 0){
              System.out.println("Missing port number! Try any number between 1024 to 49151");
              return;
          }

          int port = Integer.parseInt(args[0]);

          Server.start(port, new Handler());
      }
    }
`

The method in my code that is called is handleRequest. It took in the URI "localhost:4020/add-message?s=Hello". The relevant values are "Hello", this gets added to an arraylist, which was initially empty, that stores the string and prints it out. 

![hello](https://user-images.githubusercontent.com/122561998/215376070-c7406ccb-1436-469a-9a9b-b77709fd34cb.PNG)

The method in my code that is called is handleRequest. It took in the URI "localhost:4020/add-message?s=How are you". The relevant values are "How are you", this gets added to an arraylist, which already contained the string "Hello", and then gets printed out or returned.

![how are u](https://user-images.githubusercontent.com/122561998/215376087-39645d09-9103-42d3-a9a5-fcb4e884a7d5.PNG)

## Part 2 - Bugs

The bug I chose is in the ArrayExamples class in the method reverseInPlace. This piece of code induces a failure.
'

    @Test 
	public void testReverseInPlace2() {
        int[] input2 = {11,22,33};
        ArrayExamples.reverseInPlace(input2);
        assertArrayEquals(new int[]{33,22,11}, input2);
	}
        
'

This piece of code does not produce a failure.
'

    @Test 
        public void testReverseInPlace() {
            int[] input1 = {11};
            ArrayExamples.reverseInPlace(input1);
            assertArrayEquals(new int[]{11}, input1);;
        }
    
'

This is what happens when I run both tests.

![run](https://user-images.githubusercontent.com/122561998/215655144-5b0aabc0-7da0-4c91-a8c7-fd066ae76530.PNG)

Before the change to fix it:
'

      static void reverseInPlace(int[] arr) {
        for(int i = 0; i < arr.length; i += 1) {
          arr[i] = arr[arr.length - i - 1];
        }
      }
  
'

After the code change. This fixes the problem as it is able to use the orginal values of the array to properly reverse them rather than trying to reverse the array with the new, reversed values.
'

    static void reverseInPlace(int[] arr) {
        int[] temp = new int[arr.length];
        for(int i = 0; i < arr.length; i += 1) {
          temp[i] = arr[arr.length - i - 1];
        }
        arr = temp;
      }

'

## Part 3 - Something New I learned
I knew next to nothing about building and running a web server. When I did it in lab 2, it was my first time doing so. I learned how to use the URLHandler interface from the number incrementing activity and was able to apply that same knowledge to create the StringServer. Also, I learned that doing Ctrl-c could stop the server as well as any terminal command that's an infinite loop.

![default](https://user-images.githubusercontent.com/122561998/215657284-c263df3f-da29-482c-8933-485753bf0493.PNG)

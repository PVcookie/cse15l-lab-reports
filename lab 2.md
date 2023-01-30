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
The method in my code that is called is handleRequest,
![hello](https://user-images.githubusercontent.com/122561998/215376070-c7406ccb-1436-469a-9a9b-b77709fd34cb.PNG)

![how are u](https://user-images.githubusercontent.com/122561998/215376087-39645d09-9103-42d3-a9a5-fcb4e884a7d5.PNG)

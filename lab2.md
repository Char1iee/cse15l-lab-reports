# CSE15L Lab Report Charlie Shang
## Lab 2 Report
```
import java.io.IOException;
import java.net.URI;


class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String words = "";
    int count = 0;

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return words;
        } else if (url.getPath().contains("/add-message")) {
            String[] parameters = url.getQuery().split("=");
            if (parameters[0].equals("s")) {
                count += 1;
                words += (count + ". " + parameters[1] + "\n");
                return words;
            } else {
                return "wrong argument";
            }
        } else {
            return "404 Not Found!";
        }

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
```
![Image](add_message_1.png)<br />
* Method `handleRequest` in the class `Handler` is called when I add `add-message` to the url. Method `main` in the class `StringServer` is called to start the server.
* The argument of `handleRequest` is a url which is the url of the website.
![Image](add_message_2.png)<br />

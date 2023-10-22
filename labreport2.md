# Lab Report 2

```
import java.io.IOException;
import java.net.URI;


class Handler implements URLHandler {

    int num = 0;

    public String handleRequest(URI url) {
        if (url.getPath().contains("/add")) {
            String[] parameters = url.getQuery().split("=");
            for (int i = 0; i < parameters.length; i++) {
                System.out.println(parameters[i]);
            }
            if (parameters[0].equals("s")) {
                num += 1;
                return (num + ". " + parameters[1] + "\n");    
            }
            return "404 Not Found!";
        }
        return "";
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
![Image](Hello.png)
![Image](How.png)



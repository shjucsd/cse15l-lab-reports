# Lab Report 2 - Servers and Bugs

* ## Part 1 - StringServer


**Code**

![Image](stringserver.jpg)

**Output 1**

![Image](o1.jpg)

**Output 2**

![Image](o2.jpg)
1. In both the cases, the main method inside StringServer class is called which starts a server with the port number provided in the command line input by the user. 
2. After ther server is started, we can click on the link provided in the command line which would be something similar to `http://localhost:port`
3. After going to the server, we can edit its path and add `/add-message?string we want to display` to the path. This would call the handleRequest function in the code which will update the message to be displayed on the server's page.
4. In the first output, it is the first time editing the path so it just displays the message value which I provided as input for 's ='. Hence, the `msg` variable in code is relevant. If I had not typed anything after the path, the 'msg' variable would remain unchanged and the website would display nothing. However, since I include 'add=message' command, it gets edited path by using the 'getPath' method and then calls 'getQuery' method along with split() to access the value I provided. At last, it concatenates the provided value to 'msg' variable along with a new line character(\n) and returns it which gets displayed on the page. 
5. Similarly, for the second output as well. The 'msg' variable holds relevance. It calls the same methods - getPath, get Query, split - to get the other value I provided. But this time, it adds to the existing value of 'msg' which had been changed in output 1. It concatenates the provided value to that which leads to the display of both 'Hi' and 'How are you'. 

* ## Part 2 - Debugging

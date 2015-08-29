---
title: Using Curl to Test Backend Routes
---

using curl in the command line allows you to imitate the front-end sending requests to the backend, so you can check if routes are acting as expected.

To imitate a POST request you can use a template similar to curl --data "varName=value&varName2=value2" localhost:8080/route. where the string represents properties attached to the request body and multiple properties are seperated by the &. It is important to not use spaces in this long string unless for a properties string value that should contain a space or spaces. the localhost:8080/route can be replaced with wherever you are running your server. In this case I am making a request to localhost on port 8080 and the path is /route.

A GET request that requires the request body to have properties would follow the same template as above. If no properties are needed, the --data "" can be omitted. Thus leaving curl localhost:8080/route.

You can use these curl requests to help you find out if you correctly set up routes and/or database.




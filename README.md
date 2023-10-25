# edatesting

**There are 2 rulebook currently around webhook testing:**
- webhook.yml
    - This rulebook will listen to port 5000 and respond to the event payload of event. Using Hello! will say one thing while anything else will give a different response
- webhook-debug.yml
    - This rulebook listens to port 6000 and just prints out what json data is sent to it. This is helpful to see what your program sends to automate off of


**how to send a webhook using curl:**
- Using the CLI to post data:
 -curl --header "Content-Type: application/json" --request POST --data '{"message":"Hello!"}' http://(EDA-controller):6000
- Using a file to post data:
 -curl --header "Content-Type: application/json" --request POST --data @event.json http://(EDA-controller):6000



Ref: https://github.com/cloin
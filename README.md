# tutorial
In this tutorial I Created a deployment Spec that creates a simple nginx application with an init container 
(containers that run before the main container runs with your containerized application) .

init container role is to run git clone to a specific github repo and mount it to our EmptyDir volume everytime before our main container starts.

the outcome is that whenever a new container starts he will start with my most recent committed repo .

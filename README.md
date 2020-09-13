                                                                     tutorial

In this tutorial I Created a deployment Spec that creates a simple nginx application with a volume type EmptyDir and an init container (containers that run before the main container runs with your containerized application) .

The init container role is to clone a git repository to our EmptyDir volume every time before our main container starts.

The outcome is that whenever a new container starts he will start with my most recent committed repo mounted in his filesystem .



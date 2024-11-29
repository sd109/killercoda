### Part 2

A customer is trying deploy a new app on their Kubernetes cluster.

They have asked you for some help with troubleshooting the application deployment and have provided the set of Kubernetes manifests which comprise their app. These have been placed in the `~/app` folder inside your environment.

Start by listing the resources which make up customer's app:

```
ls ~/app
```{{exec}}

Next, try installing the app on the target cluster:

```
kubectl apply -f ~/app
```{{exec}}

Did the app deploy successfully?

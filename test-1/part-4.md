### Success criteria

The customer has told you that when the application is working correctly, it should be possible to reach their website using a Kubernetes port-forward.

To set up a port-forward run the following command:

```
kubectl port-forward svc/customer-app 80
```{{exec}}

With this port-forward still running, open a the second terminal tab and run

```
nc -vz localhost 80
```{{exec}}

If the customer's app is running correctly, you should see `Connection to localhost 80 port [tcp/http] succeeded!`

Can you figure out what's wrong with their app?

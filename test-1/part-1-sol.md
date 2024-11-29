### Part 1

Start by exploring the environment using the `kubectl` command. Here are some suggestions for questions you may want to answer:

- How many nodes does this Kubernetes cluster have?

**Solution:** `kubectl get nodes`{{exec}} (hint: click on the command to run it in the terminal)

- Which version of Kubernetes is it running?

**Solution:** *See previous output*

- How many pods are running on the cluster?

**Solution:** `kubectl get pods -A`{{exec}}

**Follow up question:** What does the `-A` do? How might you find out if you don't know?

<br>

### Extra challenges

- How might you extract the `kubeconfig` file for the cluster?

**Solution:** `kubectl config view --raw`{{exec}}

**Alternative Solution:** Any `kubectl` command in extra verbose mode with `-v6` e.g. `kubectl get nodes -v6`{{exec}}

- What is the IP address of each cluster node?

**Solution:** `kubectl get nodes -o wide`{{exec}}

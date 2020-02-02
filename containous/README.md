## Example of a minimal cluster

This uses the `containous` image to demonstrate multiple pods and ingress.

Some tests you might run include:

* change the number of replicas
* manually `kubectl delete pod <podname>` and watch kubernetes start a new one
* change the pod and ingress ports

Note:

* the `containous` image is available for both x86_64 and armv7 so it runs in VirtualBox/Vagrant on a Windows PC, as well as on a pi4

### To test

Connect a web browser to http://<your_k3s_master> port 80 and see which agent host responds

### To run

kubectl apply -f setup.yaml

### To delete

kubectl delete -f setup.yaml

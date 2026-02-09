# k8s_Practical_test

### K8S MCQ 

Q1. What is the smallest unit that Kubernetes deploys?
A. Node
B. Pod
C. Service
D. Container

Ans: B) pod

Q2. Which Kubernetes object is used to expose pods to network traffic?
A. Pod
B. Deployment
C. Service
D. Namespace

Ans: c) service

Q3. Which Service type is used only for internal communication inside the cluster?
A. NodePort
B. LoadBalancer
C. ClusterIP
D. ExternalName

Ans: c)  ClusterIP

Q4. You want to access an application using <NodeIP>:<Port> 
Which Service type should you use?
A. ClusterIP
B. NodePort
C. LoadBalancer
D. Headless

Ans: B) NodePort


Q5. Which Service type is mainly used in cloud environments to expose
applications externally?
A. ClusterIP
B. NodePort
C. LoadBalancer
D. ExternalName

Ans: c) LoadBalancer

Q6. A pod is deleted accidentally. Which pod type can automatically recreate it?
A. Standalone Pod
B. Static Pod
C. Pod managed by Deployment
D. Init Pod

Ans: c) Pod managed by Deployment

Q7. Which pod type is used to run initialization tasks before the main container
starts?
A. Sidecar Pod
B. Init Pod
C. Static Pod
D. Multi-container Pod

Ans: B) Init Pod


Q8. Containers inside the same pod communicate using:
A. Different IP addresses
B. Service only
C. Same IP address
D. External LoadBalancer

Ans: C) Same IP address

Q9. Which Service assigns a stable internal IP address automatically?
A. NodePort
B. LoadBalancer
C. ClusterIP
D. ExternalName

Ans: C) ClusterIP 

Q10. You created a Service, but traffic is not reaching the pod.
What is the most common reason?*-DCEX
A. Wrong image
B. Label mismatch
C. Pod crash
D. Node failure

Ans: B) Label mismatch

Q11. Which Kubernetes component provides DNS-based service discovery?
A. kubelet
B. kube-proxy
C. CoreDNS
D. Scheduler

Ans: C. CoreDNS

Q12. You want a pod to always run on a specific node.
Which pod type is used?
A. Init Pod
B. Sidecar Pod
C. Static Pod
D. Ephemeral Pod

Ans: C) Static Pod

Q13. Which Service type exposes a fixed port on every node?
A. ClusterIP
B. NodePort
C. LoadBalancer
D. ExternalName

Ans: B) NodePort

Q14. You want pods inside the cluster to access an application using a DNS name.
Which Service type should you use?
A. NodePort
B. LoadBalancer
C. ClusterIP
D. ExternalName

Ans: C) ClusterIP 

Q15. Which command shows the IP address of a pod?
A. kubectl get nodes
B. kubectl logs pod
C. kubectl get pods -o wide
D. kubectl describe service

Ans: D) kubectl get pods -o wide

Q16. You created a LoadBalancer Service in a local cluster.
What usually happens?
A. External IP is assigned immediately
B. External IP stays pending
C. Pod is deleted
D. Service creation fails

Ans: 

Q17. Which pod type is commonly used to support a main application with logging
or monitoring?
A. Init Pod
B. Standalone Pod
C. Sidecar Pod
D. Static Pod

Ans: C) Sidecar Pod

Q18. Which Service field decides which pods receive traffic?
A. ports
B. type
C. selector
D. metadata

Ans: C) selector

Q19. Which command is used to list all Services in a namespace?
A. kubectl get pods
B. kubectl get svc
C. kubectl describe pod
D. kubectl logs svc

Ans: B) kubectl get svc

Q20. Two pods in the same namespace want to communicate.
What is the recommended Kubernetes way?
A. Use pod IP directly
B. Use Service name
C. Use node IP
D. Use external IP

Ans: A) Use pod IP directly

#### Practical Assignment 
## Task:
You are given an application image that runs a web server.
Perform the following steps:

1.Create a Deployment that runs the application with at least 2 pods.
## Application Output Screenshot

![Browser Output](Screenshort/cmd.png)


2.Ensure all pods are created successfully and are in Running state.
3.Create a NodePort Service to expose the application.
4.Access the application from a browser using:
     http://<NodeIP>:<NodePort>
5.Verify that the application output is visible in the browser.
6.Take a screenshot of the browser output.

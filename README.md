This repository contains the resources for a hands-on lab from the course Introduction to Containers with Docker, Kubernetes & OpenShift, part of the ***IBM DevOps and Software Engineering Professional Certificate.*** The lab demonstrates how to Deploying a StatefulSet. 

A StatefulSet manages the deployment and scaling of a set of pods, and maintains a sticky identity for each of their Pods, ensuring that each Pod has a persistent identity and storage.

The lab emphasizes deploying workloads where order, stable network identity, and state persistence are critical.

***Overview***

This hands-on lab guides users through the process of how to use a StatefulSet in Kubernetes to manage the deployment of pods . 

***Learning Objectives**

***By completing this lab, you will:**
    • Understand the purpose and functionality of Kubernetes StatefulSets.
    • Learn how to configure and deploy a StatefulSet.
    • Manage persistent storage for stateful applications.

***Technologies Used***
    • Kubernetes
    • Docker
    • YAML
    • kubectl (Kubernetes CLI)

***Prerequisites***

Before starting this lab, ensure you have:
    • A working Kubernetes cluster (e.g., Minikube, MicroK8s, or a cloud provider's Kubernetes service).
    • kubectl installed and configured to communicate with your cluster.
    • Basic knowledge of Kubernetes concepts (Pods, Deployments, and Services).

***Steps to Run the Lab***

***1.Clone the repository***

git clone https://github.com/marioscloud/deploying_statefulset_kubernetes

***2. Open the file named statefulset.yaml in edit mode and check the code.***

   vim statefulset.yaml

***3. Apply the StatefulSet configuration. ***

    kubectl apply -f statefulset.yaml
This command tells Kubernetes to create the resources defined in the YAML file. 

***4. Verify that the StatefulSet is created. ***

    kubectl get statefulsets

After applying the StatefulSet, you should verify that the StatefulSet has been created and is running. This can be done using the kubectl get command.
By following these steps, you can successfully apply a StatefulSet in Kubernetes. The kubectl apply command is used to create the StatefulSet, and the kubectl get command helps you verify that the StatefulSet is running as expected.

***Contributing***
Contributions are welcome! Feel free to submit issues or pull requests to improve the lab or documentation.

***License***
Distributed under the MIT License. See LICENSE for more details.

***Acknowledgements***
Thanks to the contributors IBM DevOps and Software Engineering Team

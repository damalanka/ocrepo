# ocrepo
A Repo for OpenShift 

This is trial and error for creating git repo for OpenShift.

Thanks one and all for all your spport.

1. What is OpenShift and it's architecture. 

OpenShift is an enabler for microservice architectures, while also supporting more traditional workloads. Many organizations will also find OpenShift native features sufficient to enable a DevOps process, while others will find it is easy to integrate with both standard and custom Continuous Integration/Continuous Deployment tools.

   Openshift Architecture.

![OCarc](https://user-images.githubusercontent.com/43290241/117357380-7f7a0380-aed2-11eb-8a65-69f2302bf64d.PNG)


The Open Shift architecture employs master servers that manage node servers that run applications as containers.

OpenShift provides additional authentication, security, scheduling, networking, storage, logging, metrics, and application life-cycle management over default Kubernetes features.

Open Shift provides built-in high availability (HA) for masters and pods.

2. How it is different from v3 to v4.

OpenShift 3 - manually following reference guides (yes, you need to install it using ssh, yum, vim and other old-school tools) or with openshift-ansible project. The latter is probably a better choice, but since it needs to be universal and it’s written in Ansible it’s a little bit slow, complex and hard to troubleshoot. It does come with a major feature coveted by enterprise environments - rolling-update of the whole cluster. This is a major advantage and you will probably appreciate it when you decide to upgrade your Kubernetes cluster.

OpenShift 4 - has a simplified and easier to use installer that currently supports AWS and vSphere. It is performed by a dedicated Operator software and the whole configuration is kept in ConfigMaps inside a cluster (not in files on master servers like in version 3). Bare metal installations are still possible but currently they require many manual steps. Also it requires internet connections so disconnected installations are unavailable.

![OCP4](https://user-images.githubusercontent.com/43290241/117361989-5b212580-aed8-11eb-8dc8-8fd428c817b1.PNG)

![OCP3and4](https://user-images.githubusercontent.com/43290241/117362990-94a66080-aed9-11eb-8388-d100b9473390.PNG)



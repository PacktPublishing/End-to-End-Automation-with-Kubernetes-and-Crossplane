
### Get this product for $5

<i>Packt is having its biggest sale of the year. Get this eBook or any other book, video, or course that you like just for $5 each</i>


<b><p align='center'>[Buy now](https://packt.link/9781801811545)</p></b>


<b><p align='center'>[Buy similar titles for just $5](https://subscription.packtpub.com/search)</p></b>


# End to End Automation with Kubernetes and Crossplane
<a href="https://www.packtpub.com/cloud-networking/end-to-end-automation-with-kubernetes-and-crossplane?utm_source=github&utm_medium=repository&utm_campaign=9781801811545"><img src="https://static.packt-cdn.com/products/9781801811545/cover/smaller" alt="Early Access" height="256px" align="right"></a>

This is the code repository for [End to End Automation with Kubernetes and Crossplane](https://www.packtpub.com/cloud-networking/end-to-end-automation-with-kubernetes-and-crossplane?utm_source=github&utm_medium=repository&utm_campaign=9781801811545), published by Packt.

**Develop a control plane-based platform for unified infrastructure, services, and application automation**

## What is this book about?
In the last few years, countless organizations have taken advantage of the disruptive app deployment operating model provided by Kubernetes. With the launch of Crossplane, the same benefits are coming to the world of infrastructure provisioning and management. The limitations of Infrastructure as Code with respect to drift management, role-based access control, team collaboration, and weak contract are making people move toward control-plane-based infrastructure automation, but setting it up requires a lot of know-how and effort. 

This book covers the following exciting features:
* Understand the context of Kubernetes-based infrastructure automation
* Get to grips with Crossplane concepts with the help of practical examples
* Extend Crossplane to build a modern infrastructure automation platform
* Use the right configuration management tools in the Kubernetes environment
* Explore patterns to unify application and infrastructure automation
* Discover top engineering practices for infrastructure platform as a product

If you feel this book is for you, get your [copy](https://www.amazon.com/dp/1801811547) today!

<a href="https://www.packtpub.com/?utm_source=github&utm_medium=banner&utm_campaign=GitHubBanner"><img src="https://raw.githubusercontent.com/PacktPublishing/GitHub/master/GitHub.png" 
alt="https://www.packtpub.com/" border="5" /></a>

## Instructions and Navigations
All of the code is organized into folders. For example, Chapter03.

A block of code is set as follows:
```
# List all resources
kubectl api-resources

# List resources in the "apps" API group
kubectl api-resources --api-group=apps

# List resources in the "networking.k8s.io" API group
kubectl api-resources --api-group=networking.k8s.io
```
Any command-line input or output is written as follows:
```
% kubectl get all -n crossplane-system
helm delete crossplane --namespace crossplane-system
```

**Following is what you need for this book:**
This book is for cloud architects, platform engineers, infrastructure or application operators, and Kubernetes enthusiasts who want to simplify infrastructure and application automation. A basic understanding of Kubernetes and its building blocks like Pod, Deployment, Service, and Namespace is needed before you can get started with this book.

With the following software and hardware list you can run all code files present in the book (Chapter 1-11).
### Software and Hardware List
| Software required | OS required |
| ------------------------------------ | ----------------------------------- |
| Kind Kubernetes cluster - v1.21.1 | Windows, Mac OS X, and Linux (Any) |
| Crossplane -v.15.0 (minimum Kubernetes v1.16.0) |  |
| Helm v3.8.0 (minimum Kubernetes v3.0.0) |  |
| GCP Crossplane provider - v0.18.0 |  |
| AWS Crossplane provider - v0.23.0 |  |

We also provide a PDF file that has color images of the screenshots/diagrams used in this book. [Click here to download it](https://packt.link/1j9JK).

<!-- 

-->
## Errata

* Page 184,185: Command examples should be **"vela addon"** instead of "vela add-on"

<!-- 

-->

### Related products
* The Kubernetes Bible [[Packt]](https://www.packtpub.com/product/the-kubernetes-bible/9781838827694?utm_source=github&utm_medium=repository&utm_campaign=9781838827694) [[Amazon]](https://www.amazon.com/dp/1838827692)

* Continuous Delivery with Docker and Jenkins - Third Edition [[Packt]](https://www.packtpub.com/product/continuous-delivery-with-docker-and-jenkins/9781803237480?utm_source=github&utm_medium=repository&utm_campaign=9781803237480) [[Amazon]](https://www.amazon.com/dp/1803237481)

## Get to Know the Author
**Arun Ramakani**
is a passionate distributed platform development and a technology blogging expert living in Dubai, a dynamic city where many cultures meet. He is currently working as a Technology Architect at PwC, specializing in Evolutionary Architecture Practices, Kubernetes DevOps, Cloud-Native Apps, and Microservices. He has over a decade of experience working in a variety of different technology, domain, and teams. He has been part of many digital transformation journeys in the last few years. This book is an inspiration from one of his recent works. He is enthusiastic about learning in public and committed to helping individuals in their cloud-native learning journey.


### Download a free PDF

 <i>If you have already purchased a print or Kindle version of this book, you can get a DRM-free PDF version at no cost.<br>Simply click on the link to claim your free PDF.</i>
<p align="center"> <a href="https://packt.link/free-ebook/9781801811545">https://packt.link/free-ebook/9781801811545 </a> </p>
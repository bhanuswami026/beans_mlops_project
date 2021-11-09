# beans_mlops_project
An end-to-end image classification model with deployment in GCP along with CI/CD

### ABOUT THE ML MODEL:
Beans is a dataset of images of beans taken in the field using smartphone cameras. It consists of 3 classes: 2 disease classes and the healthy class. Diseases depicted include Angular Leaf Spot and Bean Rust. 

![alt text](https://github.com/AI-Lab-Makerere/ibean/blob/master/bean-example-data.png)
Data was annotated by experts from the National Crops Resources Research Institute (NaCRRI) in Uganda and collected by the Makerere AI research lab.

The goal is to build a robust machine learning model that is able to distinguish between diseases in the Bean plants. Beans are an important cereal food crop for Africa grown by many small-holder farmers - they are a significant source of proteins for school-age going children in East Africa.

The data is of leaf images representing 3 classes: the healthy class of images, and two disease classes including Angular Leaf Spot and Bean Rust diseases. The model should be able to distinguish between these 3 classes with high accuracy. The end goal is to build a robust, model that can be deployed on a mobile device and used in the field by a farmer.

The data includes leaf images taken in the field. The figure above depicts examples of the types of images per class. Images were taken from the field/garden a basic smartphone.

The images were then annotated by experts from NaCRRI who determined for each image which disease was manifested. The experts were part of the data collection team and images were annotated directly during the data collection process in the field.

Class	            Examples
Healthy class	        428
Angular Leaf Spot	    432
Bean Rust	            436
Total:	              1,296
Data can be downloaded from here: https://github.com/AI-Lab-Makerere/ibean/

### CI DEFINED:
Continuous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day. Each check-in is then verified by an automated build, allowing teams to detect problems early. By integrating regularly, you can detect errors quickly, and locate them more easily.

The integration happens after a “git push,” usually to a master branch—more on this later. Then, in a dedicated server, an automated process builds the application and runs a set of tests to confirm that the newest code integrates with what’s currently in the master branch.

CI works in three simple stages: push, test, and fix. But despite this simplicity, CI might become challenging if only a few members of the team practice it. Consequently, CI also requires a change in culture and support from management.

#### TOOLS FOR CI:
CI is mainly a cultural shift, but some tools could help you to get the job done quickly.
* Jenkins—a free, open-source, Java-based tool that gives you a lot of flexibility.
* Azure Pipelines—a Microsoft product free for up to five users and open-source projects.
* Cloud Build—the managed service offering from Google Cloud Platform.
* AWS cloud build.
* Travis CI—a popular tool for GitHub open-source projects that offers a hosted or self-hosted solution.
* GitLab CI—a free tool from GitLab that can also integrate with other tools via the API.
* CircleCI—a tool that’s popular for GitHub projects and has a hosted and self-hosted solution. You can start for free.
* CodeShip—a self-hosted-only solution. You can start with the free version, but it’s a paid tool.

### CD DEFINED:
Continuous Delivery is the ability to get changes of all types—including new features, configuration changes, bug fixes and experiments—into production, or into the hands of users, safely and quickly in a sustainable way. We achieve all this by ensuring our code is always in a deployable state, even in the face of teams of thousands of developers making changes on a daily basis.

#### PRINCIPLES OF CD:
* Frequent Small deployments
* Automation with a human touch
* Always improving
* Shared responsibility model

#### TOOLS FOR CD:
* Jenkins—can also be used for CD with its pipeline as code, Ansible, or Terraform plugins.
* Azure Pipelines—has a release definition section that you can integrate with a build stage from CI.
* Spinnaker—gaining popularity, and it’s the tool that Netflix uses to do releases in a CD way.
* GitLab CI—lets you configure deployment and release pipelines with GitLab.
* GoCD—the ThoughtWorks offering that applies the principles I’ve discussed in this post.


### IMPLEMENTING CI/CD PIPELINES WITH KUBERNETES AND SERVERLESS ARCHITECTURES:
Many teams operating CI/CD pipelines in cloud environments also use containers such as Docker and orchestration systems such as Kubernetes. Containers allow for packaging and shipping applications in standard, portable ways. Containers make it easy to scale up or tear down environments that have variable workloads.

Serverless computing architectures present another avenue for deploying and scaling applications. In a serverless environment, the infrastructure is fully managed by the cloud service provider and the application consumes resources as needed based on its configuration. On AWS for example, serverless applications run as Lambda functions and deployments can be integrated into a Jenkins CI/CD pipeline with a plug-in. 

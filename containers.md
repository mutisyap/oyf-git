# How to learn containers
By Peter Mutisya

## The process
1. Understand software unit of distribution
   - Compiled vs interpreted languages
     - Understand which languages need to be compiled and which one don't need to.
   - Understand what will be running:
     - We code on .java files, but we may want to run jar files.
       - Check different between Jar and war files.
     - We code on .c or .cpp files but you may want to deploy .exe files.
   - Software packaging: The process of building an installer that includes application resources to be used to distribute to distribute.
     - Packaging in Java Maven (.jar, war)
     - Packaging for Windows (.exe)
     - Packaging for Debian Linux (.deb)
     - Packaging for Android (.apk)
   - Building and recompiling software: Here, we code in a non-compliant way, then we have to change it back to a compliant way. This is very common with frameworks.
    - Building Angular (ng build): Build to Html, CSS and JS files
    - Building React (npm build) : Build to Html, CSS and JS files
    - Recompiling Typescript to JavaScript
    - Building PHP Laravel: Back to PHP compliant files.
   - Resources:
     - https://www.advancedinstaller.com/what-is-software-packaging.html
     - https://www.baeldung.com/cs/compiled-vs-interpreted-languages
     - https://www.educative.io/blog/compiled-vs-interpreted-language
     - https://www.freecodecamp.org/news/compiled-versus-interpreted-languages/
2. How to run web applications (Applications accessible on the internet)
   - What is a server
   - Understanding VMs
   - Understand embedded servers.
   - Setting up runtime dependencies
     - Java: 
       - Install open jdk
     - Web:
       - Install Apache
   - Understanding root folder for web pages.
     - Apache: /var/www/html
     - Nginx:  /usr/share/nginx/html
   - Understanding configurations: What is it that can change when running the application in different environments.
   - Resources:
     - https://www.springboottutorial.com/java-programmer-essentials-what-is-an-embedded-server
     - https://realtimelogic.com/articles/What-is-an-Embedded-Application-Server
     - https://nginx.org/en/
     - https://httpd.apache.org/
     - https://kinsta.com/knowledgebase/what-is-nginx/
     - https://www.geeksforgeeks.org/difference-between-jdk-and-jre-in-java
     - https://www.geeksforgeeks.org/differences-jdk-jre-jvm/
     - https://www.nakivo.com/blog/physical-servers-vs-virtual-machines-key-differences-similarities/
     - 
3. Read about containers
   - https://www.freecodecamp.org/news/a-beginner-friendly-introduction-to-containers-vms-and-docker-79a9e3e119b/
   - https://medium.com/geekculture/introduction-to-containers-basics-of-containerization-bb60503df931
   - https://www.docker.com/resources/what-container/

4. Understanding Docker:
   - History of Docker
   - Docker components
   - Docker Commands
     - Build image
     - List images
     - Run container
     - List containers
   - Docker Hub
     - Create docker hub
     - Push container to docker hub
     - Pull container
     - Docker login
   - Docker run
     - Mapping files
     - Mapping ports
     - Docker networking model
   - Resources:
     - https://docs.docker.com/
5. Container orchestration
   - Understand orchestration. What is it, and why is it needed
   - Understand different solutions for orchestration.
   - Understanding Kubernetes
     - What does it do, what can it not do?
     - Understand what Openshift Container Platform is.
   - Resources
     - https://www.parallels.com/blogs/ras/container-orchestration/
     - https://kubernetes.io/docs/tutorials/kubernetes-basics/
     - https://www.ibm.com/cloud/blog/openshift-vs-kubernetes
6. Kubernetes: Basic commands
   - Install MicroK8s on your laptops
     - Run basic kubernetes commands
     - Deploy a service there
   - Kubernetes on the cloud
     - Places where you can start your free cluster:
       - https://labs.play-with-k8s.com/
       - https://labs.play-with-k8s.com/
       - https://training.play-with-kubernetes.com/
     - Natujenge official cluster:
       - This will be provided to you during the week.
   - Resources:
     - https://kubernetes.io/docs/setup/
     - https://medium.com/swlh/local-cluster-vs-remote-cluster-for-kubernetes-based-development-6efe2d9be202
     - https://loft.sh/blog/development-in-kubernetes-local-vs-remote-clusters/

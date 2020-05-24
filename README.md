# Spring-cloud-service-registration-and-discovery
This repo guides you through the process of starting and using the Netflix Eureka service registry.

In the cloud, applications can’t always know the exact location of other services. A service registry, such as Netflix Eureka, or a sidecar solution, such as HashiCorp Consul, can help. Spring Cloud provides DiscoveryClient implementations for popular registries such as Eureka, Consul, Zookeeper, and even Kubernetes' built-in system. There’s also a Spring Cloud Load Balancer to help you distribute the load carefully among your service instances.

## In case you find a bug/suggested improvement for Spring Restfull Webservices
Our issue tracker is available here: https://github.com/Sudarshan-Gowda/Spring-cloud-Service-registration-and-discovery/issues

## Working with Rest in Eclipse

### prerequisites
The following items should be installed in your system:
* Tool - STS(Spring Toot Suite) or Eclipse (Optional*)

### Steps:

1) Download this Project and do maven import.
```
git clone https://github.com/Sudarshan-Gowda/Spring-cloud-Service-registration-and-discovery.git
```
2) To Import the Praject Using STS or Eclipse.
```
File -> Import -> Maven -> Existing Maven project
```

## Steps to test the application:

1) Once the application is installed properly, Run as Java Application if you are using in Eclipse, STS or any other tool.
2) The application should be run based on the order of <b>eureka-service-app</b> then <b>eureka-client-app</b>
3) If you are not using any tools to import and run the application means alternatively you can do by using below commands if thr maven plugin is already installed means,
   <ol>
    <li>Go to the project directoy of /eureka-service-app and execute the command in terminal `mvn spring-boot:run` </li>
    <li>Go to the project directoy of /eureka-client-app and execute the command in terminal `mvn spring-boot:run` </li>
   </ol>
4) The eureka-client defines a Spring MVC REST endpoint (ServiceInstanceRestController) that returns an enumeration of all the    registered ServiceInstance instances at http://localhost:8080/service-instances/a-bootiful-client. <br>
   <img src="https://github.com/Sudarshan-Gowda/Spring-cloud-Service-registration-and-discovery/blob/master/docs/Pic1.png" width="100%"/>
5) You can check the resistry by using below url http://localhost:8761/ <br>     
   <img src="https://github.com/Sudarshan-Gowda/Spring-cloud-Service-registration-and-discovery/blob/master/docs/Pic2.png" width="100%"/>
   
## User reference or guide.
  https://spring.io/guides/gs/service-registration-and-discovery/
  
# Contributing

The [issue tracker](https://github.com/Sudarshan-Gowda/Spring-cloud-Service-registration-and-discovery/issues) is the preferred channel for bug reports, features requests and submitting pull requests.


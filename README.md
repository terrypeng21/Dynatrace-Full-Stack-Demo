# Setup OneAgent monitoring in your environment

This repository contains a step-by-step guide for your introductory steps and best-practices in achieving full-stack observability with Dynatrace. 

# What is full-stack monitoring in Dynatrace?
Dynatrace full-stack monitoring offers a comprehensive view of the entire application stack, including both infrastructure and application layers. This includes the application code, databases, APIs, and user experience as well as insights into end-to-end performance, including response times, error rates, and dependencies between different components.

### Pre-requisites

* Dynatrace Managed/SaaS Account
  * Get your free 15-day SaaS trial account [here](https://www.dynatrace.com/signup/)
* Host server and application to monitor
  * List of extensive technologies supported by the OneAgent [here](https://docs.dynatrace.com/docs/ingest-from/technology-support#technology-support)

### 1) Deploy Dynatrace
Download and install OneAgent on your host

1. Go to **Search** > **Deploy OneAgent**.
2. Select the platform you're going to monitor.
![alt_text](https://github.com/terrypeng21/Dynatrace-Full-Stack-Demo/blob/main/images/Step%201%20OA.png)

4. Follow the Deployment steps for the platform you're monitoring.
   >For this guide I have chosen to install my OneAgent on a Linux Virtual Machine
![alt_text](https://github.com/terrypeng21/Dynatrace-Full-Stack-Demo/blob/main/images/Step%202%20install%20OA.png)
5. Create the Download token and store it in a safe location/password manager
   >Leave the default "Full-stack" monitoring mode as we will need it for full-stack monitoring of our environment.
6. (**Optional**) Set the customized options for your host-groups, network zones and tags to plan the deployment of multiple entities. This will not be covered in this guide as we will be monitoring a single host
7. Download the installer and run it with **root** rights (steps 2-4 in the documentation)
   >If there are strict firewall/network policies in place, you will need to whitelist the IPs found on the bottom of this page, such as this:
![alt_text](https://github.com/terrypeng21/Dynatrace-Full-Stack-Demo/blob/main/images/firewall%20policy.png)

8. Installation will be complete when you see a message like this:
![alt_text](https://github.com/terrypeng21/Dynatrace-Full-Stack-Demo/blob/main/images/Step%204%20Install%20OA.png)

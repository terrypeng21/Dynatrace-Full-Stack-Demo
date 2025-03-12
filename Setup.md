# Setup OneAgent and ActiveGate (optional) monitoring in your environment

This repository contains a step-by-step guide for your introductory steps and best-practices in achieving full-stack observability with Dynatrace. 

# What is full-stack monitoring in Dynatrace?
Enter text here

### Pre-requisites

* Dynatrace Managed/SaaS Account
  * Get your free 15-day SaaS trial account [here](https://www.dynatrace.com/signup/)
* Host server and application to monitor
  * List of extensive technologies supported by the OneAgent [here](https://docs.dynatrace.com/docs/ingest-from/technology-support#technology-support)

### 1) Deploy Dynatrace
Download and install OneAgent on your host

1. Go to **Search** > **Deploy OneAgent**.
2. Select the platform you're going to monitor.


3. Follow the Deployment steps for the platform you're monitoring.
   >For this guide I have chosen to install my OneAgent on a Linux Virtual Machine

4. Create the Download token and store it in a safe location/password manager
   >Leave the default "Full-stack" monitoring mode as we will need it for full-stack monitoring of our environment.
5. (Optional) Set the customized options for your host-groups, network zones and tags to plan the deployment of multiple entities
   >This will not be covered in this guide as we will be monitoring a single host
6. Download the installer and run it with **root** rights (steps 2-4 in the documentation)
   >If there are strict firewall/network policies in place, you will need to whitelist the IPs found on the bottom of this page, such as this:
   >Installation will be complete when you see a message like this:

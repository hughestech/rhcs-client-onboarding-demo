Process Driven Client Onboarding Application
============================================
Welcome to the Process Driven Application -  Client Onboarding Demo developed in conjunction with Red Hat JBoss BPM 
Suite and Entando running on OpenShift Container Platform. This demo illustrates a large number of process-driven use 
cases and  highlights a client-centric user experience with JBoss BPM Suite. 

Some features of this demo include: Case management, drag-n-drop application building, smart inbox, document 
approvals/attachments, custom task screens, PDF viewers, decision management, analytics, forms, and digitized 
processes.

This demo automates the installation of the process driven application for client onboarding in the Cloud based on 
OpenShift Container Platform. It delivers a fully functioning client onboarding example containerized on OpenShift
Container Platform.


Install Process Drive Client Onboarding on OpenShift
----------------------------------------------------
1. First ensure you have an OpenShift container based installation, such as one of the followling installed first:

  - [OCP Install Demo](https://github.com/redhatdemocentral/ocp-install-demo)

  - [Red Hat Container Development Kit (CDK) using Minishift](https://developers.redhat.com/products/cdk/overview)

  - or your own OpenShift installation.

2. [Download and unzip this demo.](https://github.com/redhatdemocentral/rhcs-client-onboarding-demo/archive/master.zip)

3. Run 'init.sh', 'init.bat' or 'init-win10.bat' file (.bat files must be run with Administrative privileges):
```
   # The installation needs to be pointed to a running version
   # of OpenShift, so pass an IP address such as:
   #
   $ ./init.sh 192.168.99.100  # example for OpenShift Container Platform
```

See next section for how to run through this demo.


Running demo
------------
There is a [demo script detailing how to run this demo](https://github.com/redhatdemocentral/rhcs-client-onboarding-demo/raw/master/docs/client_onboarding_demo_script.pdf), it includes some of the log in details, for logging in to the client onboarding to start exploring a process driven application (the addresses will be generated by the init script):

  - OpenShift Container Platform examples: 

    ```
    http://entando-fsi-backoffice-client-onboarding.192.168.99.100.nip.io/fsi-backoffice

         ( u:account / p:adminadmin )
         ( u:knowledge / p:adminadmin )
         ( u:legal / p:adminadmin )
         ( u:Manager / p:adminadmin )
    
    http://entando-fsi-customer-client-onboarding.192.168.99.100.nip.io/fsi-customer
    ```
Instructions for running this demo are in [this demo script.](https://github.com/redhatdemocentral/rhcs-client-onboarding-demo/raw/master/docs/client_onboarding_demo_script.pdf)


Note before running demo:
-------------------------

Should your local network DNS not handle the resolution of the above address, giving you page not found errors, you can apply the
following to your local hosts file:

```
$ sudo vi /etc/hosts

# add host for OCP demo resulution
192.168.99.100   entando-fsi-backoffice-client-onbaording.192.168.99.100.nip.io 
192.168.99.100   entando-fsi-customer-client-onbaording.192.168.99.100.nip.io 
```

-----

This project can be installed on any OpenShift platform, such as OpenShift Container Platform.
It's possible to install it on any available installation by pointing this installer to an OpenShift IP address:
```
  $ ./init.sh IP
```

-----

If for any reason the installation breaks or you want a new installation, just remove the project entry in the OpenShift console and re-run the installation.


Supporting Articles
-------------------
Coming soon...


Released versions
-----------------
See the tagged releases for the following versions of the product:

- v1.0 - Process driven application for client onboarding intalled on any OpenShift Container Platform 3.7 using process server 6.4.

[![Docs](https://raw.githubusercontent.com/redhatdemocentral/rhcs-client-onboarding-demo/master/docs/demo-images/docs.png?raw=true)](https://github.com/redhatdemocentral/rhcs-client-onboarding-demo/raw/master/docs/client_onboarding_demo_script.pdf)

![FSI Backoffice](https://raw.githubusercontent.com/redhatdemocentral/rhcs-client-onboarding-demo/master/docs/demo-images/fsi-backoffice-ui.png?raw=true)

![FSI Customer](https://raw.githubusercontent.com/redhatdemocentral/rhcs-client-onboarding-demo/master/docs/demo-images/fsi-customer-ui.png?raw=true)

![Deployment](https://raw.githubusercontent.com/redhatdemocentral/rhcs-client-onboarding-demo/master/docs/demo-images/ocp-deployment.png?raw=true)

![Cloud Suite](https://github.com/redhatdemocentral/rhcs-client-onboarding-demo/blob/master/docs/demo-images/rhcs-arch.png?raw=true)


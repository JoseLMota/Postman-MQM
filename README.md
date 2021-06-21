**REST API TO ANSIBLE PLAYBOOK**


**TEST EXAMPLE MQ REST API**


# <span id="anchor"></span>MQ Administration using the REST API or Other Software

You can use the administrative REST API to administer IBM® MQ objects,
such as queue managers and queues, and Managed File Transfer agents and
transfers. Information is sent to, and received from, the administrative
REST API in JSON format. These RESTful APIs can help you to embed IBM MQ
administration into popular DevOps and automation tooling.

Also as an application developer.

![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/mqrestapi.png)

Idea:

To create a full ANSIBLE Collection for MQSeries using the funcionality
REST API.

Steps for Solution:

  - Create a Postman full JSON Collections and Environments
    specification to test and execute code (

https://github.com/emea-ansible-automation-summit/solution-restapitoansible/tree/main/Postman

**Postman MQ ENV**


![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/mqenv.png)


**Postman MQ Collection**


![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/mqcollection.png)



  - Generate ANSIBLE playbooks.

**The list of code generators for POSTMAN are:**

![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/postmancode.png)

![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/postmantestmq.png)

**Why don’t we generate code for ANSIBLE?**

**I created a  wrapper to translate CURL source code output into
ANSIBLE-PLAYBOOK with URI module.**

![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/curltoansible.png)

Generated code
 
![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/code.png)


Playbook Output

![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/outputansilbe.png)

 


**So, in theory all REST API can be transformed into ANSIBLE-PLAYBOOK
with this converter.**


**Also tested Ansible-Tower and vcenter REST-API ansible generator with Postman Collection**

**Postman AWX public collection in postman rep**

**Postman vcenter public collection in postman rep**

![](https://github.com/emea-ansible-automation-summit/solution-restapitoansible/blob/main/images/awxpostmancollection.png)

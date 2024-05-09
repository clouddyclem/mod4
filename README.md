Module 4 for SES homework

![AWS Architecture Diagram (2)](https://github.com/clouddyclem/mod4/assets/169360868/c35c0c6b-ab20-421d-9d10-0a51c9dcdbdc)

The 3 tier web application architecture consists of:
  (1) Front-end that hosts the user interface,
  (2) Back-end that processes data, and
  (3) Database for data storage and management.

This design is able to achieve the well-architected framework with high availability.

**Operational Excellence:**
By hosting the front end, backend and database tiers seperately, components can be updated in small, frequent and reversible changes with different teams/individuals working on the respective components. 
Operational events are also easily monitored for analysed to achieve operational success. Timely drills can also be carried out for operational teams to be familiar with disaster recovery procedures and ensure that the procedures in place are feasible.

**Security**
By segregating each tier with its own security groups, security measures and whitelisting can be customized to suit the business needs. Since security is of paramount importance, it is best practice for least privileges to be given to only those who need it. Constant review on IAM roles and permissions should be carried out to ensure that least privileges are given. Network traffic should also be denied by default and only whitelisting through specific IP addresses should be done. On top of that, WAF and intelligent threat detection services such as AWS Guard duty should also be used to prevent any malicious attacks.

**Performance Efficiency**
Having a good understanding of the CSP's services and capabilities would help when it comes to architecture selection. Configuration of the autoscaling policies would require planning and analysis to enable optimal efficiency in scaling fo resources. Predictive workloads can be planned in advance in order to reduce any impact on the application.

**Reliability**
This design is reliable with multi-az deployments with autoscaling enabled. This will help to automatically recover from failure and deploying in multi-az will prevent downtime in the event of a data center wide outage. This can be further enhanced to multi region deployments, taking into consideration the geolocation data regulations as well as cost.

**Cost Optimization**
This can be achieved by consistently monitoring the utilization of resources and plan for right-sizing appropriately in order to save cost.

**Sustainability**
Maximizing resources and minimizing wastage of computing resources will in turn help to reduce power wastage that would cause an impact to the environment.

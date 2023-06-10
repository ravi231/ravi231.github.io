---
layout: post
title:  "OCI Create A User To Access Sreaming Service"
date:   2023-06-03 10:38:06 +0530
categories: [oracle_cloud_infrastructure, OCI_SIEM_Integration]
tags: [OCI, OCI_Kafka_Streaming, SIEM, Audit]
---


# OCI Integration with SIEM through Kafka Streaming Services - Part 1

## Creating a User and Providing Permission to Access OCI Streaming Services.

### 1. Under “Identity and Security” select “Identity”

![Desktop View](/assets/img/OCI/1.png){: width="700"}

### 2. Click on domain. 

![Img2](/assets/img/OCI/2.png){: width="700"}

### 3. Create a New User.

![Img3](/assets/img/OCI/3.png){: width="700"}

![Img4](/assets/img/OCI/4.png){: width="700"}
 
### 4. Create a Auth Token for this user.

![Img5](/assets/img/OCI/5.png){: width="700"}
 
### 5. Copy the Generated auth token.

### 6. Create a Group and make the user part of the group.

![Img6](/assets/img/OCI/6.png){: width="700"}

![Img7](/assets/img/OCI/7.png){: width="700"}
 
### 7. Create a Policy.

![Img8](/assets/img/OCI/8.png){: width="700"}
 
### 8. While creating the policy , select “policy usecases” as “Streaming” and select highlighted “common policy template” as per below screenshot.

![Img9](/assets/img/OCI/9.png){: width="700"}

### 9. Assign “Groups” we created earlier to this policy and select the “Location”. 
 
Make a note of Username and Auth token , It will be required while configuring Kafka consumer to pull the logs from OCI Streaming Services.





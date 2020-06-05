+++
weight = 1
+++

{{% section %}}

# Connecting to Docker Container

![](/images/docker/docker-connect.png)

---

### 1. Connect to Remote Machine
<br/>
From **local machine** connect to **remote machine** first:

<br/>
```
ssh username@10.10.10.10

 
ssh -i mykey.pem username@10.10.10.10
```
<br/>
(Using remote host's IP/DNS, and cryptographic key if available.)

---

### 2. Connect to Docker Container
<br/>
From **remote machine** connect to **docker container** running:

<br/>
```
docker exec -it container_id bash
```
<br/>
(Use `docker ps` for running Docker containers, and its id.)

{{% /section %}}

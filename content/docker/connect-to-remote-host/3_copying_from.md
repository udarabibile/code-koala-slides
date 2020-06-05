+++
weight = 3
+++

{{% section %}}

# Copying from Docker Container


![](/images/docker/docker-copy-from.png)

---

### 1. Copy to Remote Machine
<br/>
From **docker container** copy to **remote machine** first:

<br/>
```
docker cp container_id:/container/file/app.log /file/path/ 


docker cp container_id:/container/directory/path/. /directory/path/
```
<br/>
(Use `docker ps` for running Docker containers, and its id.)

---

### 2. Copy to Local Machine
<br/>
From **remote machine** copy to **local machine** running:

<br/>
```
scp username@10.10.10.10:/remote/file/path /local/file/path

 
scp -P 3000 username@10.10.10.10:/remote/directory/path/* /local/directory/path/


scp -r username@10.10.10.10:/remote/directory/path /local/directory/path
```
<br/>
(Copy files or directories to given location in local using applicable flags for recursive or port.)

{{% /section %}}

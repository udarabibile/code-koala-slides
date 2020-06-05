+++
weight = 2
+++

{{% section %}}

# Copying to Docker Container


![](/images/docker/docker-copy.png)

---

### 1. Copy to Remote Machine
<br/>
From **local machine** copy to **remote machine** first:

<br/>
```
scp /local/file/path username@10.10.10.10:/remote/file/path

 
scp -P 3000 /local/directory/path/* username@10.10.10.10:/remote/directory/path


scp -r /local/directory/path username@10.10.10.10:/remote/directory/path
```
<br/>
(Copy files or directories to given location in remote using applicable flags for recursive or port.)

---

### 2. Copy to Docker Container
<br/>
From **remote machine** copy to **docker container** running:

<br/>
```
docker cp /file/path/note.txt container_id:/container/file/path


docker cp /directory/path/. container_id:/container/directory/path
```
<br/>
(Use `docker ps` for running Docker containers, and its id.)

{{% /section %}}

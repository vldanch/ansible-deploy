Web app back docker build:
```yml
docker build -t vldanch/kubia .
```
Install docker to remote hosts:
```yml
ansible-playbook -i hosts playbook.yml --tags docker-install -kK
```
Install docker apps to remote host:
```yml
ansible-playbook -i hosts playbook.yml --tags apps-install -kK
```

Checking the container from the host:
```yml
curl localhost:8080

Output of the coneiners id: 
You've hit 3de9d62c875c
```
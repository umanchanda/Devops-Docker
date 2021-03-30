```sudo docker run --name logs devopsdockeruh/exec_bash_exercise```

```sudo docker exec -it logs sh```

Inside the terminal:

```tail -f ./logs.txt```

Secret message: ```"Docker is easy"```
# Game of Pods Solution
## Links
K8s [course](https://www.udemy.com/course/certified-kubernetes-application-developer) reference.
Practice environment [Game of Pods](https://kodekloud.com/courses/game-of-pods/).

## Game of Pods
The game is composed by some broken k8s environments, and is used to train k8s knowledge, once solved the tasks, you may receive a token. 
The token is than used to resolve the broken environments on the Game.

## Project Structure
Each folder on this repo represents an environment on Game of Pods. Not all the environments are opened for playing with, so I will just solve the ones I have access to.

## How it was done
I first tried to solve the problems writing by hand all the yamls, with the help of `kubectl explain <resource>`. Yeah crazy... but I was doing this trying to understand everything.
Than I tried one next try using the reference from [k8s official documentation](https://kubernetes.io/);
And one last try using the imperative commands, all the files in here will use an alias `k` for the command `kubectl`.
[Here](https://kubernetes.io/docs/reference/kubectl/cheatsheet/#bash) you may found how to set the alias.

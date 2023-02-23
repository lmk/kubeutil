# kubeutil
kubernetes utils 

## features

- Displays the current context at the bash prompt.

- kexecti: execute a command inside a container

```
host> $ kexecti my-pod ls -l
total 4
-rw-r--r-- 1 root root 82  Feb 23 10:32 README.md
```

- kexecsh: Connect to the container with a bash shell

```
host> $ kexecsh my-pod
pod> $ 
```

- klogf: Print the container's logs.
```
host> $ klogf my-pod
```


## usage
include .bash_profile

```bash
source .kubeutil
```

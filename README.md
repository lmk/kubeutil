# kubeutil
kubernetes utils 

If input part of the pod name after the alias, it will find that pod and perform the command.
If there are multiple matching pods, it will output a list of candidates.

## features

- Displays the current context at the bash prompt.

- kexecti: execute a command inside a container

  - same ```kubectl exec -ti -n my-namespace my-pod -- ls -l```

```
host> $ kexecti my-pod ls -l
total 4
-rw-r--r-- 1 root root 82  Feb 23 10:32 README.md
```

- kexecsh: Connect to the container with a bash shell

  - same ```kubectl exec -ti -n my-namespace my-pod -- bash --login```

```
host> $ kexecsh my-pod
pod> $ 
```

- klogf: Print the container's logs.

  - same ```kubectl logs -f -n my-namespace my-pod```

```
host> $ klogf my-pod
```


## usage
include .bash_profile

```bash
source .kubeutil
```


### Start a new pod
k run my-pod-name --image=name-of-pod-image-i-want

### Get running pods
k get pods
k get pods -o wide  (gets more details)

### Get pod yaml
k get pod nginx

### Describe a pod
k describe pods/nginx

### Describe all pods
k describe pods

### Edit Pod
k edit pod nginx

### Dryrun a Pod (to get the yaml)
k run nginx --image=nginx --dry-run=client -o yaml

### Create a pod from YAML
-  k create -f myfile.yaml
	- Only creates
- k apply -f myfile.taml
	- Creates or applies changes to running pod with same name

### Execute into a Pod
k exec -it nginx-docs -- /bin/bash

Note: bash may not be available; try sh / posix shell otherwise

Press CTRL-D to get out of the interactive session

### Delete a pod
k delete pod nginx


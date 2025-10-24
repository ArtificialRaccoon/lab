
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


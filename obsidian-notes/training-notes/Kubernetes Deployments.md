### Create a simple deployment

k create deploy test --image=httpd --replicas=3

k create deploy test --image=httpd --replicas=10 --dry-run=client -o yaml > deploy.yaml
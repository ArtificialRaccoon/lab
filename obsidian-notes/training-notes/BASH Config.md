Add the following to the .bashrc
Then call source ~./bashrc (or just logout)

~~~
# Kubectl

alias k='kubectl'

source /etc/bash_completion
source <(kubectl completion bash)
complete -o default -F __start_kubectl k
~~~

Allows for autocomplete, and also creates an alias (k) for faster input.
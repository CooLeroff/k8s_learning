This is repository of learning cources K8S

**Tips & trics**

Plugin for VSC to editing - YAML editor from RedHat
Configurating:
In settings, find settings.json and add section:
```
{
    "yaml.schemas": {

        "kubernetes" : ["*.yml","*.yaml"]

    },
```

**Autocompliete Kubectl in Linux (Bash shell)**

Install
```
apt-get install bash-completion
```
Enable autocomplete by add script in ./bashrc
```
echo 'source <(kubectl completion bash)' >>~/.bashrc
```
Reload bash
```
source ~/.bashrc
```
Use nano editor to edit kubectl (for example "replicaset")

```
KUBE_EDITOR="nano" kubectl rs replicaset
```
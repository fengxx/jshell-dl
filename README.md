## usage
download busybox to /tmp/busybox and link /tmp/bin/sh to /tmp/busybox

```
# download it
cat jshell_dl.txt |kubectl exec -i pod-name -n namespace -- jshell --execution local  -
# using the sh
kubectl exec -it pod-name -n namespace -- /tmp/bin/sh
# inside the debug sh
export PATH=/tmp/bin/:$PATH
```

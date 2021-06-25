`cat /etc/kubernetes/manifests/kube-apiserver.yaml`

openssl x509 -in /etc/kubernetes/pki/apiserver.crt -text -noout

do this for kube-controller, etcd, scheduler etc.

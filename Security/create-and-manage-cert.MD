access granting proces

![image](https://user-images.githubusercontent.com/17488415/123401901-d774e280-d5c4-11eb-9c35-b034ee9bf919.png)

1. create user cert `openssl genrsa -out amit.key 2048`
2. create CSR `openssl req -new -key amit.key -subj "/CN=jane" -out amit.csr` 
3. encode CSR `cat amit.csr |base64`

```yml
# amit.yaml
apiVersion: certificates.k8s.io/v1beta1
kind: CertificateSigningRequest
metadata:
  name: amit
spec:
  groups:
  - system:authenticated
  usages:
  - digital signature
  - key encipherment
  - server auth
  request:
    <certificate-goes-here>
```
4. `kubectl create -f amit.yaml`
5. list the csr `kubectl get csr`
6. Approve the request `kubectl certificate approve amit`
7. View the certificate `kubectl get csr amit -o yaml`
8. Decode it `echo "<certificate>" |  base64 --decode`


![image](https://user-images.githubusercontent.com/17488415/123402987-f0ca5e80-d5c5-11eb-805b-b5f3c46e4610.png)

# kubernetes-traefik-ingress-controller
Code required to install a traefik ingress controller in kubernetes 1.24

---

<b>apply traefik-api.yaml</b>  
kubectl apply -f traefik-api.yaml

<b>apply pv and pvc</b>
Traefik needs somewhere to store certificates and keys where they will persist on traefik pod recreation.  
Below uses longhorn as the storage provider and host path.  

kubectl apply -f traefik-pv.yaml  
kubectl apply -f traefik-pvc.yaml  

c

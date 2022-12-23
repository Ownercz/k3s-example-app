---
apiVersion: extensions/v1beta1
kind: Ingress
metadata:
  name: k3s-demo
#  annotations:
#    kubernetes.io/ingress.class: "traefik"

spec:
  rules:
  - host: k3s-node1.lipovcan.cz
    http:
      paths:
      - path: /
        backend:
          serviceName: k3s-demo
          servicePort: http

---
apiVersion: extensions/v1beta1
kind: Ingress
metadata:
  name: k3s-demo
  annotations:
    kubernetes.io/ingress.class: "traefik"

spec:
  rules:
  - host: k3s-demo.example.org
    http:
      paths:
      - path: /
        backend:
          serviceName: k3s-demo
          servicePort: http

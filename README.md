# Kubernetes Multi-Tier Deployment

This project demonstrates deployment of frontend and backend applications on Kubernetes using:

- Namespaces
- Resource Quotas
- Node Labels
- Taints
- Node Selectors
- Deployments
- Services (NodePort and ClusterIP)

## Architecture

Internet
    |
 NodePort
    |
Frontend Pod (node2)
    |
 ClusterIP
    |
Backend Pod (node3)

## Features

- Frontend deployed on dedicated worker node
- Backend deployed on separate worker node
- Frontend exposed using NodePort
- Backend exposed internally using ClusterIP
- Separate namespaces for isolation
- Resource quotas applied to each namespace

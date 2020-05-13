# One-node-cluster

## Okey, it's simply for situations, when you need all-in-one cluster

## What will it do:

 - Install docker through get-docker script
 - Switch docker-directory home folder to directory "new_home" from hosts-file
 - Switch docker to use systemd
 - Add insecure registry to your docker daemon-json(by default it will be)
 - Disable firewall
 - Disable SELinux
 - Disable swap
 - Install kubelet, kubectl, kubeadm
 - Bootstrap cluster
 - Deploy Calico CNI to the cluster
 - Deploy traefik 1.7 with self-signed SSL-cert and WS/WSS support
 - Deploy k8dash as your dashboard
 - Create cronjob for updating control-plane certs each 3 month

## Features:

 - You can use it behind closed network, if you have proxy(just mention it in hosts-file)
 - You can switch user added to docker group from root in hosts-file(user should be exist)

## Versions:

 - Calico: 3.14
 - Traefik: 1.7

## Possible updates: 

 - Deploy docker-registry
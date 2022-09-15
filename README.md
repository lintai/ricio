# ricio
RIC depends on some k8s

## k8s部署相关镜像
部署k8s,./install_k8s_and_helm.sh缺失的镜像
coredns  
etcd  
kube-apiserver  
kube-controller-manager  
kube-proxy  
kube-scheduler  
pause
./install_common_templates_to_helm.sh，安装网络插起前检查pod发现缺失的镜像  
mirrored-flannelcni-flannel  
mirrored-flannelcni-flannel-cni-plugin
quay.io_coreos_flannel

## RIC相关的镜像
./install -f ../RECIPE_EXAMPLE/example_recipe_latest_stable.yaml 需要的镜像15个  
it-dep-secret:0.0.2  
ric-plt-a1:2.5.1  
ric-plt-alarmmanager:0.5.11  
it-dep-init:0.0.1  
ric-plt-appmgr:0.5.4  
ric-plt-e2mgr:5.4.19  
ric-plt-e2:5.5.0  
ric-plt-o1:0.5.3  
ric-plt-rtmgr:0.8.2  
ric-plt-submgr:0.8.2  
ric-plt-vespamgr:0.7.5  
kubernetes-ingress-controller:0.7.0  
alertmanager:v0.20.0  
prometheus:v2.18.1  
ric-plt-dbaas:0.5.5  
tiller:v2.16.12
configmap-reload:v0.3.0
kong:1.4

## xapps
chartmuseum/chartmuseum:v0.12.0
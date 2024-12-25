

PS C:\Users\balag\.kube\ArgCD> mkdir my-helm


PS C:\Users\balag\.kube\ArgCD> cd .\my-helm\

PS C:\Users\balag\.kube\ArgCD\my-helm>  git clone { clone the git repo}
  Ex: git clone https://github.com/NaveenBalagouni/my-helms-charts.git

PS C:\Users\balag\.kube\ArgCD\my-helm>  cd git repo


PS C:\Users\balag\.kube\ArgCD\my-helm> helm create my-helm-chart
Creating my-helm-chart

PS C:\Users\balag\.kube\ArgCD\my-helm> ls

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        05-11-2024     11:29                my-helm-chart


PS C:\Users\balag\.kube\ArgCD\my-helm> helm package my-helm-chart
Successfully packaged chart and saved it to: 

C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart-0.1.0.tgz


PS C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart>
 helm repo index . --url https://NaveenBalagouni.github.io/my-helm-charts


C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart> git add 
          
              git add -A

               git commit -m "Add Helm chart and index.yaml"

              git push origin 







my-helm-repo/
├── charts/
│   └── my-chart/
├── my-helm-repo-0.1.0.tgz
└── index.yaml




 

PS C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart\my-helm-charts> 

helm repo add my-helm-charts https://raw.githubusercontent.com/NaveenBalagouni/my-helm-charts/main/




PS C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart\my-helm-charts> helm repo index . --url https://raw.githubusercontent.com/NaveenBalagouni/my-helm-charts/main/


PS C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart\my-helm-charts>
 helm repo add my-helm-charts https://raw.githubusercontent.com/NaveenBalagouni/my-helm-charts/main/
{"my-helm-charts" has been added to your repositories}


git add -A

 git commit -m "edite"

git pull
.

git push



PS C:\Users\balag\.kube\ArgCD\my-helm\my-helm-chart\my-helm-charts> helm repo update



PS C:\Users\balag\.kube\ArgCD\my-helm-repos\my-helm-repo> helm search repo 

my-helm-repo
NAME                            CHART VERSION   APP VERSION     DESCRIPTION
my-helm-chart-repo/my-helm-repo 0.1.0           1.16.0          A Helm chart for Kubernetes
my-helm-repo/my-helm-repo       0.1.0           1.16.0          A Helm chart for Kubernetes


# DevOps
cd /opt
    2  git clone http://54.214.113.35:9090/test/CustomerMgmt.git
    3  yum install git
    4  git clone http://54.214.113.35:9090/test/CustomerMgmt.git
    5  ls -ltr
    6  cd CustomerMgmt
    7  ls -ltr
    8  cd ..
    9  git clone http://34.212.188.131/dipankar/kubernetes.git
   10  ls -ltr
   11  cd kubernetes
   12  ls -ltr
   13  cd masterscript
   14  ls -ltr
   15  ./cluster-setup.sh
   16  aws configure
   17  ls -ltr
   18  ./cluster-setup.sh
   19  kops validate cluster
   20  kubectl cluster-info
   21  ls -ltr
   22  ./prerequisite.sh
   23  kubectl get pods -n devops
   24  kubectl describe pod artifactory-k8s-deployment-66f548b58f-lmbcb -n devops
   25  ls -ltr
   26  ./install.sh
   27  ls -al
   28  cat install.sh
   29  helm --version
   30  whereis helm
   31  export PATH=$PATH:/usr/local/bin/
   32  helm --version
   33  helm list
   34  sudo yum install docker
   35  docker version
   36  service docker status
   37  service docker start
   38  docker version
   39  ./install.sh
   40  kubectl get pods --all-namespaces
   41  kubectl get pods -n jenkins-masters -owide
   42  kubectl cluster-info
   43  kubectl get nodes -owide
   44  cat ~/.kube/config
   45  ls v-al
   46  ls -al
   47  cat cluster-setup.sh
   48  cat ~/.bashrc
   49  cat ~/.bash_profile
   50  source ~/.bash_profile
   51  rm -rf kubernetes
   52  ls -ltr
   53  cd /opt
   54  ls -ltr
   55  rm -rf kubernetes
   56  rm -rf CustomerMgmt
   57  kubectl get pods
   58  kubectl get deployment
   59  kubectl get svc
   60  ls -ltr
   61  vi phoenix
   62  cd phoenix
   63  ls -ltr
   64  cd yaml
   65  ls -ltr
   66  vi dep.yaml
   67  cp service.yaml service_coe.yaml
   68  ls -ltr
   69  vi service_coe.yaml
   70  kubectl create -f service_coe.yaml
   71  vi service_coe.yaml
   72  kubectl create -f service_coe.yaml
   73  kubectl get svc
   74  kops validate cluster
   75  cat install.sh
   76  cat ../referscript/deploy-k8s-dashboard.sh
   77  echo 'DASHBOARD CREDENTIALS: '$(kops get secrets kube --type secret -o plaintext)
   78  echo 'DASHBOARD TOKEN: '$(kops get secrets admin --type secret -o plaintext)
   79  echo 'ACCESS DASHBOARD --> https://'$(kubectl get nodes -owide | awk '/master/{print $6}')'/api/v1/namespaces/kube-system/services/https:kubernetes-dashboard:/proxy/'
   80  kubectl get pods --all-namespaces
   81  cd ../referscript/
   82  ls -al
   83  ./deploy-k8s-dashboard.sh
   84  kubectl create -f https://raw.githubusercontent.com/kubernetes/dashboard/master/aio/deploy/recommended/kubernetes-dashboard.yaml

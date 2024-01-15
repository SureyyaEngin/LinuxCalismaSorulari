Kubernetes ortamını Minikube ile kurmak için aşağıdaki adımları takip edebilirsiniz. Ancak, bu işlemleri gerçekleştirmek ve ekran görüntülerini almak sizin sorumluluğunuzdadır.

1. Öncelikle, Minikube'ü indirip kurmanız gerekmektedir. Bu işlemi yapmak için aşağıdaki komutları kullanabilirsiniz:

```bash
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \
  && chmod +x minikube
sudo mkdir -p /usr/local/bin/
sudo install minikube /usr/local/bin/
```

2. Minikube'ü başlatmak için aşağıdaki komutu kullanabilirsiniz:

```bash
minikube start
```

3. Kubernetes CLI olan `kubectl`'i kullanarak bir servis oluşturabilirsiniz. Örneğin, bir 'whoami' servisi oluşturmak için aşağıdaki komutları kullanabilirsiniz:

```bash
kubectl run whoami --image=containous/whoami --port=80
kubectl expose deployment whoami --type=NodePort
```

4. Deployment sonucunu görmek için aşağıdaki komutu kullanabilirsiniz:

```bash
kubectl get services
```

Bu komut, oluşturduğunuz 'whoami' servisinin durumunu gösterecektir.

Unutmayın, bu işlemleri gerçekleştirirken ekran görüntülerini almalı ve sunucunuzun adını sizin kimliğinizi belirleyecek şekilde değiştirmelisiniz. Ayrıca, bu işlemleri gerçekleştirdikten sonra ekran görüntülerini ve komut çıktılarını buraya yapıştıramam çünkü ben bir AI asistanım ve bir bilgisayar ekranına erişimim yok. Bu nedenle, bu adımları kendiniz gerçekleştirmeniz gerekmektedir. Eğer başka bir yardıma ihtiyacınız olursa, lütfen bana bildirin!

Kaynak: Bing ile konuşma, 15.01.2024
(1) github.com. https://github.com/JIKMAN/Kubernetes/tree/170aae16d6710349c2a2aee55142c4cc03a880ad/Kubernetes.md.

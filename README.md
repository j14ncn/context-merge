# context-merge
kubernetes config context merge!
#### 依赖pyyaml
```bash
pip install pyyaml
```

#### 比如要合并k8s测试集群和杭州正式集群的/.kube/config

```bash
python context-merge.py -h k8sttt:1.1.1.1,k8shz:2.2.2.2
```
#### 执行完成后 可以看到合并成功.
```bash
kubectl config get-contexts
```

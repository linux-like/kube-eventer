## kube-eventer    

---
[Fork from AliyunContainerService/kube-eventer](https://github.com/AliyunContainerService/kube-eventer)

Features:
* Add webhook sink exclude reasons

# How to run
```shell
go run eventer.go --source="kubernetes:https://172.17.3.131:6443?inClusterConfig=false&localKubeConfig=/Users/jian/.kube/config" --sink="webhook:https://open.feishu.cn/open-apis/bot/v2/hook/f4c57728-3cfc-4b56-9d00-3a34fe2d6e23?level=Warning&method=POST&header=Content-Type=application/json&custom_body_configmap=custom-body&custom_body_configmap_namespace=monitoring&exclude_reasons=FailedToRetrieveImagePullSecret"

```
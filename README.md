# sample-spring-boot-infrastructure

## 環境構築
```bash
$ ansible-playbook -i local playbook.yml
```

## デプロイ
`<user>`にローカルで実行するユーザを入れる
```bash
$ ansible-playbook -i local deploy --extra-vars "local_user=<user> ansistrano_release_version=`date +%Y%m%d%H%M%SZ`"
```

# sample-spring-boot-infrastructure

## デプロイ(+環境構築)
`<user>`にローカルで実行するユーザを入れる
```bash
$ ansible-playbook -i local deploy --extra-vars "local_user=<user> ansistrano_release_version=`date +%Y%m%d%H%M%SZ`"
```

## ロールバック
```bash
$ ansible-playbook -i local rollback.yml
```

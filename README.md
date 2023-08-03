## playbook

```
ansible-playbook -i hosts site.yml
```

途中 sudo password のプロンプトが出たりする

## ユーザパスワードの設定

```sh
$ mkpasswd --method=sha-512
```

↑の結果を `host_vars/<hoge>` の `password_sha512` に貼り付ける 

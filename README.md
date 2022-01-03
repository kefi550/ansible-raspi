## playbook
### 初回実行時(初期パスワード変更が求められる場合)

```
ansible-playbook -i hosts site.yml --ask-pass
```

### 初回以降

- 初回実行時に初期ユーザは削除するため、hostsの `ansible_user` を実行ユーザに書き換える

```
ansible-playbook -i hosts site.yml
```

## ユーザパスワードの設定

```sh
$ mkpasswd --method=sha-512
```

↑の結果を `host_vars/<hoge>` の `password_sha512` に貼り付ける 

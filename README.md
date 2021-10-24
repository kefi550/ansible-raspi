## 初回実行時(初期パスワード変更が求められる場合)

```
ansible-playbook -i hosts site.yml --ask-pass
```

初回以降

```
ansible-playbook -i hosts site.yml
````

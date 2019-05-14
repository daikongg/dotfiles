dotfiles
========

.files

```
$ sh install.sh
```

### `.gitconfig.local`でフォルダ毎にアカウントを分ける例

```.gitconfig.local
[includeIf "gitdir:~/src/github.com/repository"]
  path = ~/.gitconfig.repository
```

```.gitconfig.repository
[user]
  name = user_name
  email = email_adrress
```

---
layout: default
title: "Git & SSH Config"
lang: en
---

## Git & SSH Config

* You can manage multiple SSH keys for working on different repositories
* Personal/work profiles

```bash
$> cat ~/.ssh/config
    Host github.com-gchoy-vmware
        HostName github.com
        User git
        IdentityFile ~/.ssh/id_rsa

    Host github.com-personal
        HostName github.com
        User git
        IdentityFile ~/.ssh/personal_rsa

$> git clone git@github.com-gchoy-vmware:gchoy-vmware/git-102.git
$> git remote -v
   origin  git@github.com-gchoy-vmware:gchoy-vmware/git-102.git (fetch)
   origin  git@github.com-gchoy-vmware:gchoy-vmware/git-102.git (push)
```

* Your remotes will be pointed accordingly
* Git will use your SSH leys you defined in your SSH config
* Seamless and useful
* Need to remember differentiation
* May need to make changes to git config i.e. name, email etc.

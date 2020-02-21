# Git 102

Git 102 Repository for demonstrating some practical workflows with Git - [Git 102](https://gchoy-vmware.github.io/git-102/).

## Cloning

```bash
$> git clone https://github.com/gchoy-vmware/git-102.git
```

## Jekyll

### Linux

If you want to build the docs locally, you'll need to setup Jekyll in your environment - [Jekyll Installation](https://jekyllrb.com/docs/installation/).

```bash
$> cd docs
$> bundle install
$> bundle exec jekyll serve
```

### Windows

The easiest method is to download the Jekyll image for Docker:

```ps
PS> cd docs
PS> docker run --rm --label=jekyll --volume=${pwd}:/srv/jekyll -it -p 4000:4000 jekyll/jekyll jekyll serve --force_polling
```

Or simply execute `.\RunDocker.ps1` in the `docs` folder.

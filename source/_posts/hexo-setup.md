title: hexo setup
date: 2015-10-02 13:27:36
tags:
---

## setup

```
$ npm install hexo-cli -g
$ hexo init hexoblog
$ cd hexoblog
$ npm install
```

## launch

```
$ hexo server
```

access to  http://0.0.0.0:4000/


## deploy


github で

hexoblog というリポジトリを作っておく.


`_config.yml` を開いて

```
deploy:
  type: git
  repo: git@github.com:phi-jp/hexoblog.git
  branch: gh-pages
```

root を

```
root: /
```
↓
```
root: /hexoblog
```

```
$ hexo d -g
```

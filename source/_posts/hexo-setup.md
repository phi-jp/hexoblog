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


### github リポジトリを作る

github で hexoblog というリポジトリを作っておく.


### deploy 先を設定する

`_config.yml` を開いて

```
deploy:
  type: git
  repo: git@github.com:phi-jp/hexoblog.git
  branch: gh-pages
```

### ルートを設定

root を

```
root: /
```
↓
```
root: /hexoblog
```


### setup

```
$ npm install hexo-deployer-git --save
``

### deploy

```
$ hexo deploy -g
```


## Ref

- https://hexo.io/
- http://tech.admax.ninja/2014/09/11/environment-of-hexo/
- http://raimon49.github.io/2015/04/25/create-blog-with-hexo.html



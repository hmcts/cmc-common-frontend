# CMC common -frontend

This project contains common items for sharing across Civil Money Claims projects. 

## Install

Run:
```
$ yarn add @hmcts/cmc-common-frontend
```

## Nunjuck Macros

Add the macros folder of this project to your nunjucks search path:

```
nunjucks.configure([
  path.join(__dirname, '..', '..', 'views'),
  path.join(__dirname, '..', '..', '..', '..', 'node_modules', '@hmcts', 'cmc-common-frontend', 'macros'),
], {
  autoescape: true,
  express: app
})
```

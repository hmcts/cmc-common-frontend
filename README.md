# CMC common -frontend

[![Greenkeeper badge](https://badges.greenkeeper.io/hmcts/cmc-common-frontend.svg)](https://greenkeeper.io/)

This project contains common items for sharing across Civil Money Claim projects. 

#Nunjuck Macros

Copy the contents of the macros folder into your project and update your Nunjucks configuration to point to this new folder.

```
nunjucks.configure([
  path.join(__dirname, '..', '..', 'views'),
  path.join(__dirname, '..', '..', '..', 'public', 'macros'),
], {
  autoescape: true,
  express: app
})
```
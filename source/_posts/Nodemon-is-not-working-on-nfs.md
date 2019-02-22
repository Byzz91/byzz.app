---
title: NFS 환경에서 Nodemon이 정상작동 하지 않을때
---
**Vagrant**의 NFS 시스템으로 파일이 동기화되고 있을 때 `$ nodemon index.js`가 정상적으로 파일을 reload 하지 않는 경우 아래와 같은 옵션을 주어 해결한다.

### How To Fix

```bash
$ node -L index.js
```

원본 출처 [Nodemon isn't working on basic node server](https://github.com/remy/nodemon/issues/1086)
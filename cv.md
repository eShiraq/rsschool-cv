# Zubov Dmitry
 Frontend developer

### ***Contacts***

+ [**email**](mailto:evgenshiraq@gmail.com)
+ [**github**](https://github.com/eShiraq)

### ***About me***
A hardworking and inquisitive person who tries to get things done. Worked with server deployment. I am not a perfectionist, I try to complete the work in such a way that it suits the client first of all.

### ***Skills***
+ Bash
+ Terminal
+ Linux
+ VSCode
+ Git
+ Figma
+ HTML
+ CSS(BEM)
+ Javascript(React, Express)

### ***Code examples***

```
const jwt = require('jsonwebtoken');

const { NODE_ENV, JWT_SECRET, devSecret } = require('../utils/config');
const Unauthorized = require('../errors/unauthorized');

const auth = (req, res, next) => {
  const token = req.cookies.authToken;
  let payload;
  try {
    payload = jwt.verify(
      token,
      NODE_ENV === 'production'
        ? JWT_SECRET
        : devSecret,
    );
  } catch (err) {
    throw new Unauthorized('Ошибка токена');
  }
  req.user = payload;
  return next();
};

module.exports = auth;
```

### ***Education***

* **Ulyanovsk State University**
    + Applied Mathematics and Computer science

### ***Expirence***

+ Deployment of servers on OS Debian and Ubuntu
+ Pet projects

### ***Languages***

+ Russian
+ English(B1)

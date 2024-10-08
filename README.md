## Session with Nextjs and external API ExpressJs

#### What is included:
- Nextjs as front
- NodeJS Express as external API
- fetcher with auth
- Rotative accessToken and refreshToken


#### How to use:
- Clone and test
- Swap the static data with your query database

#### Install and test
```
npm i
npm run dev
```

#### Basic usage of fetcher with auth
```
import { get, post, put, remove } from "../utils/auth/";

const Component = async () => {

  // GET
  const users = await get("/api/users");
  console.log(users);

  // POST
  const user = await post("/api/users", { name: "John Doe" });
  console.log(user);

  // PUT
  const user = await put("/api/users", { name: "John Doe" });
  console.log(user);

  // DELETE
  const user = await remove("/api/users/1");
  console.log(user);

}
```

### Reources
https://github.com/nextauthjs/next-auth/issues/7558 

https://www.reddit.com/r/nextjs/comments/14sy295/nextjs_authentication_with_an_external_expressjs/

https://github.com/nextauthjs/next-auth/issues/7558#issuecomment-1915756093

https://github.com/nextauthjs/next-auth/issues/7558#issuecomment-2084773897

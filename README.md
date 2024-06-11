# Althea

Althea is a forked repository of Lucia, developed by Manifold Lab. It alters the userID to be a serial number instead of a string in the Drizzle Adapter for MySql Databases. This is to ensure that the userID is unique and can be used as a primary key in the database.

Further work will be completed for Manifold Lab's use case, including the addition of a new adapter for the Drizzle Adapter for Postgres and SQLite Databases.

# Lucia

Lucia is an auth library written in TypeScript that abstracts away the complexity of handling sessions. It works alongside your database to provide an API that's easy to use, understand, and extend.

-   No more endless configuration and callbacks
-   Fully typed
-   Works in any runtime - Node.js, Bun, Deno, Cloudflare Workers
-   Extensive database support out of the box

```ts
import { Lucia } from "lucia";

const lucia = new Lucia(new Adapter(db));

const session = await lucia.createSession(userId, {});
await lucia.validateSession(session.id);
```

Lucia is an open source library released under the MIT license, with the help of [100+ contributors](https://github.com/lucia-auth/lucia/graphs/contributors)!

## Resources

**[Documentation](https://lucia-auth.com)**

**[Join the Discord server!](https://discord.gg/PwrK3kpVR3)**

**[Examples](https://github.com/lucia-auth/examples)**

**[Changelog](https://github.com/pilcrowOnPaper/lucia/blob/main/packages/lucia/CHANGELOG.md)**

## Installation

```
npm i lucia
pnpm add lucia
yarn add lucia
```

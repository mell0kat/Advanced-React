### Tech Stack

**Frontend**
React.js

- Next.js for routing, server-side rendering
- Styled components
- React-Apollo

Apollo Client - replacement for Redux \* local state

- data fetching
- caching
- GraphQL mutations
- error and loading states

**Backend**
Prisma - graphQL database interface (CRUD API)

- schema definitions
- queried directly from yoga server

GraphQL Yoga - Express Server

- query and mutation resolvers
- custom server-side logic (credit card processing, sending emails, authentication)

### Next.js

- code-splitting
- webpack config
- server-side rendering
- pre-built pages (in production)

### styled-components

- benefit: CSS looks like normal CSS

### GraphQL

- specification for both server and client
- language-agnostic
- alternative to REST
- our backend implementation: Prisma
- our frontend implementation: Apollo
- one single endpoint
- typed
- self-documenting
- queries (fetching) & mutations (changes)

### Prisma

- open-source
- GraphQL ORM layer
- CRUD API

9. Fixing styled components flicker on server render (we are seeing a flash of unstyled HTML)

- we need CSS to be pre-rendered
- we will use custom server-side <Document/> (often used for css-in-js libraries like styled-components)
- `collectStyles` will be called in getInitialProps

# Reflection for IMY 210 Unit Assignment 3

This assignment had me develop a blog website with a Strapi backend, Nuxt frontend, and deployed it using Docker.

- Initially, I had an issue with Strapi configuration errors, whcich required adding keys to server.ts and admin.ts.
- Docker volume setup was quite tricky due to path formatting errors on my laptop. I fixed it by quoting the volume path
- The Nuxt container wouldn't start due to a missing "start" scripot in the package.json, but I made sure toi dix that.

Overall, it was a good experience and challenge to develop everything from my side, update changes using git, and then finally deploying everything using Docker to have the application run on any device.


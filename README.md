Wordpress Starter
---

By [Aaron Krauss](https://thecodeboss.dev)

A simple yet optimized container-driven Wordpress implementation.

Here is what makes it different from a base Wordpress install:

* Store the Wordpress code in a non-committed volume. The thought here is that
  you likely don't want to make changes to core wordpress, and thus don't need
  to commit any of it.
* Disable the `performance_schema` MySQL module, ironically to improve
  performance.
* Opt for and configure an Nginx web server front-end, instead of Wordpress'
  default of Apache

## To Run Locally
```
cp .env.example .env
# If desired, configure your database creds in .env

docker-compose up
```

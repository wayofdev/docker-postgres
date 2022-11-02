<br>

<div align="center">
<img width="456" src="https://raw.githubusercontent.com/wayofdev/docker-nginx/master/assets/logo.gh-light-mode-only.png#gh-light-mode-only">
<img width="456" src="https://raw.githubusercontent.com/wayofdev/docker-nginx/master/assets/logo.gh-dark-mode-only.png#gh-dark-mode-only">
</div>

<br>

<br>

<div align="center">
<a href="https://actions-badge.atrox.dev/wayofdev/docker-postgres/goto"><img alt="Build Status" src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fwayofdev%2Fdocker-postgres%2Fbadge&style=flat-square"/></a>
<a href="https://github.com/wayofdev/docker-postgres/tags"><img src="https://img.shields.io/github/v/tag/wayofdev/docker-postgres?sort=semver&style=flat-square" alt="Latest Version"></a>
<a href="https://hub.docker.com/repository/docker/wayofdev/postgres"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/wayofdev/postgres?style=flat-square"></a>
<a href="LICENSE"><img src="https://img.shields.io/github/license/wayofdev/docker-postgres.svg?style=flat-square&color=blue" alt="Software License"/></a>
<a href="#"><img alt="Commits since latest release" src="https://img.shields.io/github/commits-since/wayofdev/docker-postgres/latest?style=flat-square"></a>
</div>

<br>

# Docker Image: PostgreSQL

This image is used together with [wayofdev/docker-php-dev](https://github.com/wayofdev/docker-php-dev) and other WOD images, to create local development environment for our projects.

Has built in, enabled support for:

* UUID's — covered by uuid-ossp extension
* ULID's — implemented by [custom extension by Dave Allie](https://blog.daveallie.com/ulid-primary-keys)

If you **like/use** this repository, please consider **starring** it. Thanks!

![Screenshot](assets/screenshot.png)

## ⚙️ Development

To install dependencies and start development you can check contents of our `Makefile`

### →  Requirments

For testing purposes we use **goss** and **dgoss**, follow installation instructions on [their official README](https://github.com/aelsabbahy/goss/blob/master/extras/dgoss/README.md)

<br>

### → Building locally

Generating distributable Dockerfiles from yaml source code:

```bash
$ make generate
```

<br>

Building default image:

```bash
$ git clone git@github.com:wayofdev/docker-postgres.git
$ make build
```

To **build** image, **test** it and then **clean** temporary files run:

```bash
$ make
```

Building all images:

```bash
$ make build TEMPLATE="15-alpine"
$ make build TEMPLATE="14-alpine"
```

<br>

## 🧪 Testing

Testing default image:

```bash
$ make test
```

To test all images:

```bash
$ make test TEMPLATE="15-alpine"
$ make test TEMPLATE="14-alpine"
```

<br>

### → Code quality tools

Run **yamllint** to validate all yaml files in project:

```bash
$ make lint
```

Run hadolint to validate created Dockerfiles:

```bash
$ make hadolint
```

<br>

## 🤝 License

[![Licence](https://img.shields.io/github/license/wayofdev/docker-postgres?style=for-the-badge&color=blue)](./LICENSE)

<br>

## 🙆🏼‍♂️ Author Information

This repository was created in **2022** by [lotyp / wayofdev](https://github.com/wayofdev).

<br>

## 🫡 Contributors

<img align="left" src="https://img.shields.io/github/contributors-anon/wayofdev/docker-postgres?style=for-the-badge"/>

<a href="https://github.com/wayofdev/docker-nginx/graphs/contributors">
  <img src="https://opencollective.com/wod/contributors.svg?width=890&button=false">
</a>

<br>


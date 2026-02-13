# LAUNCHKIT-RS

![Rust](https://img.shields.io/badge/rust-1.75-orange)

**scaffolding generator for new projects**

you know how `cargo new` or `npm init` work? this but opinionated.

```bash
launchkit-rs new myapp --template saas
```

creates:

```
myapp/
├── backend/     (rust + actix-web)
├── frontend/    (svelte + vite)
├── db/          (postgres migrations)
├── docker-compose.yml
├── .github/workflows/
└── README.md
```

**templates available:**

- `saas` - full stack web app
- `cli` - command line tool
- `api` - rest api only  
- `game` - game engine boilerplate
- `micro` - microservice setup

**what it generates:**

- docker setup
- ci/cd pipelines (github actions)
- database migrations
- auth scaffolding (jwt via **tokenforge** lib)
- deployment configs (fly.io, railway)

**custom templates:**

```bash
launchkit-rs add-template https://github.com/user/my-template
launchkit-rs new project --template my-template
```

template format: just a git repo with `{{project_name}}` placeholders.

**alternatives:** cookiecutter (python), yeoman (node), copier (python)

**why rust?** fast. single binary. no runtime needed.

built by [@dev-scaffold](https://github.com/dev-scaffold) team during hack week.

Apache-2.0

---

> "saved me 2 hours every new project" - someone on reddit

> "templates need more variety" - valid complaint

> "windows support?" - works but untested

# PR Update: 2025-10-27 03:02:22

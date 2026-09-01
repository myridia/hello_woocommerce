# AGENTS.md — hello_woocommerce

## What this is
A starter WooCommerce setup delivered as a Docker container (Debian + Apache + PHP 8.4 + MariaDB + phpMyAdmin + WordPress CLI). Currently in planning/testing phase.

## Stack
- PHP 8.4 (Apache + mod_php)
- MariaDB
- Apache 2 with mod_rewrite
- phpMyAdmin
- Composer, WP-CLI

## Build
```bash
docker build -t hello_woocommerce .
```

## Run
```bash
./build.sh && ./run.sh
```

## Structure
- `Dockerfile` — base image, PHP/MariaDB/Apache setup
- `entrypoint.sh` — container startup script
- `phpmyadmin.conf` — phpMyAdmin Apache config
- `build.sh` / `run.sh` / `clean.sh` — build/run/cleanup helpers

## Conventions
- No comments in code unless asked.
- Verify: `php -l <file>` for PHP files.

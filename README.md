# ![app icon](./.github/readme-images/app-icon.png) Komga PostgreSQL Fork

> **⚠️ FORK NOTICE**: This is a fork of the original Komga project, modified to use **PostgreSQL 18** instead of SQLite for improved performance and scalability. This fork is **not extensively tested** and may contain bugs or lead to unexpected issues. Use at your own risk. For the official stable version, please visit the [original Komga repository](https://github.com/gotson/komga).
>
> **⚠️ DATABASE COMPATIBILITY**: 
> - This fork **requires PostgreSQL 18** and will NOT work with SQLite or other database versions
> - You **CANNOT migrate** from the original Komga's SQLite database to this PostgreSQL fork
> - You must **start from scratch** - this means re-adding your libraries and reconfiguring all settings
> - All your previous data (reading progress, collections, metadata) will be lost during migration
>
> **If you encounter any issues with this fork, please open an issue in [this repository](https://github.com/jindalpratik/komga/issues) and NOT in the original Komga repository.**

Komga is a media server for your comics, mangas, BDs, magazines and eBooks.

## Features

- Browse libraries, series and books via a responsive web UI that works on desktop, tablets and phones
- Organize your library with collections and read lists
- Edit metadata for your series and books
- Import embedded metadata automatically
- Webreader with multiple reading modes
- Manage multiple users, with per-library access control, age restrictions, and labels restrictions
- Offers a REST API, many community tools and scripts can interact with Komga
- OPDS v1 and v2 support
- Kobo Sync with your Kobo eReader
- KOReader Sync
- Download book files, whole series, or read lists
- Duplicate files detection
- Duplicate pages detection and removal
- Import books from outside your libraries directly into your series folder
- Import ComicRack `cbl` read lists

## Installation

### Using This PostgreSQL Fork

To use this PostgreSQL fork, follow these steps:

1. **Build the Docker image:**
   ```bash
   docker build -t komga:postgresql-v2 -f Dockerfile .
   ```

2. **Run with Docker Compose:**
   ```bash
   docker-compose up -d
   ```

   Make sure you have a `docker-compose.yml` file configured with PostgreSQL settings.

## Documentation

For general documentation about Komga features, refer to the [official Komga website](https://komga.org).

## Develop in Komga

Check the [development guidelines](./DEVELOPING.md).

## Credits

The Komga icon is based on an icon made by [Freepik](https://www.freepik.com/home) from www.flaticon.com

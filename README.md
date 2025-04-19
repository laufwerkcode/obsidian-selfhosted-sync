This code base creates a Docker container + Volume to run CouchDB to use as a syncing backend for [Obsidian self-hosted sync](https://github.com/vrtmrz/obsidian-livesync).

# Requierments

You will need:

- Docker
- Terraform
- Terragrunt

# Building the image

```bash
docker build ./CoucheDBContainer -t custom_obsidian_sync:v1.0
```

# Run the Grunt

```bash
terragrunt apply
```

# Troubleshooting

Did you set the right Docker socket? See `sync-module/main.tf:13`

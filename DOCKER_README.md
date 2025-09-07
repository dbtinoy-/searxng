# SearXNG Docker Setup

## Quick Start

1. **Build the Docker image:**
   ```bash
   docker build -f Dockerfile.fork -t searxng-fork:latest .
   ```

2. **Start the services:**
   ```bash
   docker-compose -f docker-compose.searxng.yml up -d
   ```

3. **Access SearXNG:**
   - SearXNG: http://localhost:8080
   - Caddy (if configured): http://localhost

## Available Dockerfiles

- `Dockerfile.fork` - Builds from your forked GitHub repository
- `Dockerfile.working` - Pre-built working version

## Configuration

- Edit `docker-compose.searxng.yml` for service configuration
- Modify SearXNG settings in the `searx/` directory (if mounted)

## Development

To make changes to SearXNG:
1. Edit files in this repository
2. Rebuild the Docker image
3. Restart the services

See `USING_SEARXNG_FORK_GUIDE.md` for detailed instructions.


# Running wild10.github.io with Docker

It looks like you want to run this project with Docker, but Docker does not seem to be installed on your system (or available in your PATH).

## 1. Install Docker

### Mac OS
1. Download **Docker Desktop** for Mac (choose Apple Silicon if you have an M1/M2/M3 chip, or Intel otherwise):
   - [Download Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Open the downloaded `.dmg` file and drag Docker to your Applications folder.
3. Open **Docker** from your Applications. You might need to grant it permissions.
4. Wait for the Docker icon in your menu bar to stop animating and say "Docker Engine is running".

## 2. Verify Installation
Open your terminal and run:
```bash
docker --version
docker compose version
```
You should see output indicating the versions.

## 3. Run the Project
Once Docker is running, you can start your website with a single command:

1. Open your terminal in the project directory:
   ```bash
   cd /Users/wilderd/Documents/website/wild10.github.io
   ```
2. Build and start the container:
   ```bash
   docker compose up --build
   ```
3. Wait for the build to finish. It might take a few minutes the first time.
4. Once you see "Server running... press Ctrl-C to stop", open your browser to:
   [http://localhost:8080](http://localhost:8080)

## Troubleshooting
- **Platform issues**: If you are on an M1/M2 Mac and see errors about architecture, try uncommenting `platform: linux/amd64` in `docker-compose.yml` (though the provided setup should work natively).
- **Gemfile.lock**: If you see errors about `Gemfile.lock`, usage of the `entry_point.sh` automatically removes it on start to avoid platform conflicts. This is normal behavior for this setup.

# Clone fork về local
git clone https://github.com/tungledjv/github-mcp-server.git
cd github-mcp-server

# Build Docker image
docker build -t tungledjv/github-mcp-server:latest .

# Push lên Docker Hub
docker push tungledjv/github-mcp-server:latest

# Hoặc push lên GitHub Container Registry
docker tag tungledjv/github-mcp-server:latest ghcr.io/tungledjv/github-mcp-server:latest
docker push ghcr.io/tungledjv/github-mcp-server:latest
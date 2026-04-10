# Solution Marius - Multi-Language Calculator APIs

This directory contains the complete solution with Docker containers for multiple calculator implementations.

## APIs

- **Go API** (Port 8090): Mathematical operations using Gin framework
- **JavaScript API** (Port 3000): Basic arithmetic operations using Express
- **Python API** (Port 4000): Trigonometric functions using Flask
- **Rust API** (Port 8000): Special endpoints using Warp framework

## Build and Run

```bash
# Build all services
docker-compose build

# Run all services
docker-compose up -d

# View logs
docker-compose logs -f

# Stop services
docker-compose down
```

## Testing the APIs

### Go API
```bash
curl http://localhost:8090/sqrt/16
curl http://localhost:8090/pow/2/10
curl http://localhost:8090/log/2.718
```

### JavaScript API
```bash
curl http://localhost:3000/add/5/3
curl http://localhost:3000/multiply/4/7
curl http://localhost:3000/divide/20/4
```

### Python API
```bash
curl http://localhost:4000/sin/1.57
curl http://localhost:4000/cos/0
curl http://localhost:4000/tan/0.785
```

### Rust API
```bash
curl http://localhost:8000/
curl http://localhost:8000/ # Call multiple times to see variation
```

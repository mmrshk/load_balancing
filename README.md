# load_balancing

```dockerfile
docker-compose down
docker-compose up -d
```

Test:
Use cURL to test the configuration with the X-Forwarded-For header set to a known US IP address:
```dockerfile
curl -H "X-Forwarded-For: 8.8.8.8" http://0.0.0.0:8080 -v
```
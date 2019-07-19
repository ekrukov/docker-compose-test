# docker-compose-test
Test file structure for docker-compose project

Each service can be run separately:

```bash
cd redis && docker-compose up -d
```

Or as one project with common network:

```bash
docker-compose up -d
```

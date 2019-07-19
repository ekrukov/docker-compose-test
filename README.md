# docker-compose-test
Test file structure for docker-compose project

Each service can be run separately:

```bash
cd redis && docker-compose up -d

Creating network "redis_test_default" with driver "bridge"
Creating test-redis ... done

docker-compose down

Stopping test-redis ... done
Removing test-redis ... done
Removing network redis_test_default
```

Or as one project with common network:

```bash
docker-compose up -d

Creating network "common_test_default" with driver "bridge"
Creating test-redis     ... done
Creating test-memcached ... done

docker-compose down 

Stopping test-memcached ... done
Stopping test-redis     ... done
Removing test-memcached ... done
Removing test-redis     ... done
Removing network common_test_default
```

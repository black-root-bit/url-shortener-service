

# 🔗 url-shortener-service

> High-performance URL shortener with custom aliases, click analytics, expiration, and Redis caching. Handles millions of redirects.

[![Java](https://img.shields.io/badge/Java-17-ED8B00?style=flat-square&logo=openjdk)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2-6DB33F?style=flat-square&logo=springboot)](https://spring.io/projects/spring-boot)
[![Redis](https://img.shields.io/badge/Redis-Cache-DC382D?style=flat-square&logo=redis)](https://redis.io)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql)](https://postgresql.org)

**Features:** Custom short codes · Expiration dates · Click count tracking · Geo & referrer analytics · Rate limiting · QR code generation · Bulk URL creation API

**Key Endpoints:**
```
POST  /api/v1/urls/shorten           # Create short URL
GET   /{code}                        # Redirect (301)
GET   /api/v1/urls/{code}/stats      # Click analytics
DELETE /api/v1/urls/{code}           # Delete URL
GET   /api/v1/urls/my               # User's URLs
```

**Performance:** Redis caches hot URLs → sub-millisecond redirect latency

**GitHub Topics:** `java` `spring-boot` `url-shortener` `redis` `postgresql` `analytics` `docker` 

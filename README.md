# mcs-ecommerce

Example microservice practice project.

## Tech Stack

**1.Observavility**: Logs (Loki,Promtail,Grafana) Metrics (Prometheus,Grafana) Traceability (OpenTelemetry,Jaeger)
**2.Database**: Relational (PostgreSQL) NoSQL (Redis) Full-text(Elasticsearch)
**3.Security**: JWT + Middleware, TLS with gRPC
**4.Testing**: Go Testing, testcontainers-go, Mockery, grpcurl
**5.CI/CD**: Docker, Helm, K8s, GitOps

## Essentials Microservices for E-commerce System

### User and security domain

| Service | Responsability |
| --- | --- |
| auth-service | Sign-in, Login, Logout, JWT, Refresh tokens, OAuth Validation |
| user-service | User profile, Shipping address, preferences |

### Product and Catalog domain

| Service | Responsability |
| --- | --- |
| product-service | Product CRUD, Stock, Description, images |
| category-service | Categories, filters, dynamice attributes |
| inventroy-service | Stock control in real time |

### Buy and Cart Shopping domain

| Service | Responsability|
| --- | ---- |
| cart-service | User persistent shopping cart |
| order-service | Order management, validation, totals, shipment |
| payment-service | Simulation or integration with payment gateway |

### Shipping domain

| Service | Responsability |
| --- | --- |
| shipping-service | Calculation of shipping costs, tracking, status, etc. |

### Comunication and Experience domain

| Service | Responsability |
| --- | --- |
| notification-service | Emails, SMS, notification push |
| review-service | Product reviews, rattings. |

### Search domain

| Service | Responsability |
| --- | --- |
| search-service | Indexing and searching |

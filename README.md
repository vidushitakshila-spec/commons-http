# commons-http

1. Problem statement: Microservices make brittle HTTP calls with inconsistent timeout configurations, missing connection pooling, and lack of standard propagation headers.

2. Concepts and terminology: RestClient, WebClient, Connection Pooling, Distributed Tracing Headers, Exponential Backoff.

3. Available technologies / algorithms: Spring Framework RestClient, Apache HttpClient 5, Resilience4j.

4. When to use what: Use as the standardized HTTP client wrapper for all synchronous service-to-service communication.

5. Java APIs and dependencies: spring-boot-starter-web, Apache HttpClient 5.

6. AWS equivalents: AWS SDK HTTP Client, API Gateway HTTP Integrations.

7. Architecture patterns: Client Interceptor Chain, Resilient Outbound Gateway, Declarative HTTP Interfaces.

8. Security considerations: Enforce strict TLS hostname verification, configure appropriate connection timeouts, and sanitize outbound URLs.

9. Implementation examples: Configured RestClient bean pre-loaded with tracing and mTLS interceptors.

10. References and further reading: Google REST API Design Guide.

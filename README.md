# spring-cloud-currency-conversion-service

---
# Readme Note 1
Test URL                : http://localhost:8100/currency-converter/from/USD/to/TRY/quantity/1000

---
# Readme Note 2
Test Feign URL          : http://localhost:8100/currency-converter-feign/from/USD/to/TRY/quantity/10

	    <dependency>
			<groupId>org.springframework.cloud</groupId>
			<artifactId>spring-cloud-starter-openfeign</artifactId>
		</dependency>
---

# Readme Note 3
Connecting currency conversion microservice to eureka

        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-eureka</artifactId>
        </dependency>
        
        @EnableDiscoveryClient
        eureka.client.service-url.default-zone=http://localhost:8761/eureka
        Open http://localhost:8761/ and see this message
        CURRENCY-CONVERSION-SERVICE 	n/a (1) 	(1) 	UP (1) - host.docker.internal:currency-conversion-service:8100
---
# Grafana and Prometheus Service

### 🕹 실행 방법

1. Docker Image 다운로드

   ```
   docker pull prom/prometheus
   
   docker pull grafana/grafana
   ```

2. Container 실행

   ```
   docker run -d -p 9090:9090 \
       --name prometheus \
       -v ./prometheus.yml:/etc/prometheus/prometheus.yml \
       prom/prometheus
    
   docker run -d -p 3000:3000 \
       --name=grafana grafana/grafana
   ```



# Monitoring Boilerplate

`Prometheus`와 `Grafana`를 통해 모니터링을 할 수 있는 프로젝트성 레포입니다.
일반적인 Spring Boot 환경 구축 뒤 모니터링과 장애대응에 대한 연습을 목적으로 합니다.

## Command

- Prometheus
```bash
docker pull prom/prometheus

docker run -d -p 9090:9090 -v /Users/{username}/Desktop/Monitoring-Boilerplate/src/main/resources/prometheus.yml:/e
tc/prometheus/prometheus.yml --name prometheus prom/prometheus
```

- Grafana
```bash
docker run -d -p 3000:3000 --name grafana grafana/grafana
```
# Thông tin triển khai ELK

## Cấu trúc thư mục 

```
elk-lab
├── docker-compose.yml
└── logstash
    └── pipeline
        └── elk-logstash.conf
```

## Các tài khoản đang được sử dụng

| Thành phần             | Tài khoản             | Mật khẩu          |
|------------------------|-----------------------|-------------------|
| Máy ảo Ubuntu          | ubuntu_elk            | 123               |
| Elastic Superuser      | elastic               | elastic!@#123     |
| Kibana System          | kibana_system         | password!@#123    |
| APM System             | apm_system            | password!@#123    |
| Logstash System        | logstash_system       | password!@#123    |
| Beats System           | beats_system          | password!@#123    |
| Remote Monitor User    | remote_monitor_user   | password!@#123    |

---

## Triển khai ELK bằng Docker
```bash
cd ~
cd elk-lab
sudo docker-compose up -d
```
---
## Truy cập Kibana 

```http://<IP_host>:5601```
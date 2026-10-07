# DevOps Hackathon - Đề 001: Quản lý phòng Lab

## 1. Thông tin sinh viên

| Họ và tên | Mã sinh viên | Lớp | Tài khoản Linux | GitHub | Cổng Nginx |
|---|---|---|---|---|---|
| Đặng Khánh An | PTIT-HN-070 | CNTT3 | `khanhanlab` | [KHANHAN007] | `8091` |

## 2. Triển khai

```bash
sudo git clone https://github.com/KHANHAN007/devops-practice-de002-khanhan007.git /var/www/devops-practice-de002-khanhan007

sudo chown -R khanhan-lab:khanhan-lab /var/www/devops-practice-de002-khanhan007

sudo find /var/www/devops-practice-de002-khanhan007 -type d -exec chmod 755 {} \;

sudo find /var/www/devops-practice-de002-khanhan007 -type f -exec chmod 644 {} \;
```

## 3. Kiểm thử

```bash
sudo nginx -t
sudo systemctl reload nginx
sudo ufw status verbose
curl -I http://127.0.0.1:8091
```

# k8s-redis-cluster

این پروژه یک نمونه ساده از اجرای Redis در Kubernetes را نشان می‌دهد. هدف آن آموزش اجرای سرویس‌های stateful ساده است.

## 📂 ساختار فایل‌ها

- `deployment.yaml`: اجرای Redis روی یک پاد
- `service.yaml`: ایجاد سرویس داخلی (ClusterIP)

## 🚀 نحوه اجرا

```bash
kubectl apply -f manifests/
kubectl exec -it <redis-pod-name> -- redis-cli

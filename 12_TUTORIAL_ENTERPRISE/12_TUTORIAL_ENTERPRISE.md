# Tutorial for Enterprise — FIXMYSTREET

**Project:** `FIXMYSTREET`
**Category:** GOVERNMENT
**Domain:** government and civic technology
**Date:** 2026-10-07

---

## Enterprise Deployment

### Pre-Deployment Checklist
- [ ] License review completed
- [ ] Security audit passed
- [ ] Compliance requirements mapped
- [ ] Support contacts established

### Deployment Options

#### Docker
```bash
docker build -t FIXMYSTREET .
docker run -p 8080:8080 FIXMYSTREET
```

#### Kubernetes
```bash
kubectl apply -f k8s/
```

#### Bare Metal
```bash
pip install FIXMYSTREET
FIXMYSTREET --config config.yaml
```

### Monitoring
- AIOSS chain for audit logging
- Prometheus metrics endpoint
- Health check at /health

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.

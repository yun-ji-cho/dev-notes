---
layout: post
title: "[Docker] 볼륨 마운트 문제 해결"
date: 2025-06-02
---

## 🧵 상황

Docker 컨테이너를 재시작하면 `/data` 폴더가 초기화됨.

## 🕵️‍♂️ 원인

볼륨 마운트 옵션이 잘못되어 로컬 디렉토리와 연결되지 않음.

## ✅ 해결 방법

```bash
docker run -v $(pwd)/data:/data my-image
```

---

# convention


# directories
## cmd
- 실제 실행 파일

```bash
cmd/foo-program/main.go
```


## configs
- 설정 파일

```bash
configs/foo-local.yaml
configs/foo-prod.yaml
```

## initialize
- 프로그램 초기 구동시 동작할 내용

```bash
initialize/env.go
```

## internal
- 프로그램 내부적으로 사용하는 파일들

### migrations
- db 마이그레이션

### models
- db 모델

### services
- db 테이블 쿼리
- 그 외 서비스

### routes
- web 서버가 있는 경우 라이터 모음


## pkg
- 외부로 서비스하거나
- 다른 프로젝트에서 공유해서 쓸만한(하지만 따로 분리하지 않은) 패키지들

### databases
- db 접속 관련

```bash
pkg/databases/mysql/mysql.go
```

### utils

```bash
pkg/utils/datetime.go
```

### api
- api 서비스를 제공하는 경우 관련 파일
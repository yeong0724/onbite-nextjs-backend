## 시작하기 (Getting Started)

### 1. 코드를 다운로드

이 저장소를 Clone 또는 Fork

### 2. 의존성 설치

```
> npm install
```

### 3. Supabse 설정

```
// .env
# Connect to Supabase via connection pooling with Supavisor.
DATABASE_URL="postgresql://postgres.uektaydysdsygkomxtuh:[YOUR-PASSWORD]@aws-0-ap-northeast-2.pooler.supabase.com:6543/postgres?pgbouncer=true"

# Direct connection to the database. Used for migrations.
DIRECT_URL="postgresql://postgres.uektaydysdsygkomxtuh:[YOUR-PASSWORD]@aws-0-ap-northeast-2.pooler.supabase.com:5432/postgres"
```

복사한 `Connection String`을 `.env` 파일을 생성하여 다음과 같이

```
// .env
DATABASE_URL="방금 복사한 Connection String"
```

</div>
</details>

### 4. 데이터베이스 스키마 설정

```
npx prisma db push
```

### 5. 시드 데이터 삽입

> (참고) 삽입되는 시드 데이터는 프로젝트 `prisma/seed/data.ts` 파일에서 확인할 수 있음

```
npm run seed
```

### 6. 서버 실행

```
> npm run build
> npm run start
```

### 7. 데이터베이스 실시간 확인

```
npx prisma studio
```

<img width="1222" alt="image" src="https://github.com/winterlood/onebite-books-server/assets/46296754/5c06d9aa-8f8b-4d9d-9763-9408e1724b13">

### 8. API 문서 확인

**http://localhost:12345/api**

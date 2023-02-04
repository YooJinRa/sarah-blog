### 프로젝트 생성

```bash
yarn create next-app blog --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"
```

### Link vs a Tag

- Link Tag를 이용하면, `Client Side Navigate`를 진행한다.
  - browser에서 url을 직접 쳐서 이동하는 것과 달리 JS 상에서 page 컴포넌트를 교체하는 것이다. 즉 데이터가 바뀐 부분만 교체된다.
- 반면에 a Tag를 이용하면, html 전체가 리로딩 된다.

### Code Splitting

- Next.js는 Automatic Code Splitting을 제공하는데, 이를 통해 성능이 최적화 된다.
  - 특정 페이지에 접근 할 때는 해당 페이지를 그릴 때 필요한 chunk만 로드한다.
  - 페이지 이동을 할 떈 목적지 페이지에 필요한 chunk만 추가 로드한다.

### Prefetching

- Viewport 내 Link 페이지를 미리 페칭한다.

### Image Component

- Resizing(responsive size)
- Lazy load(viewport에 들어오면 로드)
- 그외 optimization(webp 형태)
- CLS(Cumulative Layout Shift) : 누적 레이아웃 이동

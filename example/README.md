# JPA Examples

## JPA 사용시 주의사항

- 초기화가 모두 완료되지 않은 엔티티를 캐시하면 안 된다.  
캐시된 초기화 되지 않은 엔티티를 지연로딩으로 사용하고자 하면 `LazyInitializationException`이 발생한다.  
참고: [CacheTest](./src/test/java/cache/CacheTest.java)
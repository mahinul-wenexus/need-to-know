# What is this type declaration?
```typescript
function isValidStore(raw: unknown): raw is Store {
  return (
    raw != null &&
    typeof raw == 'object' &&
    'source' in raw &&
    typeof raw['source'] === 'string'
  );
}

// what does "raw is Store" means?
```

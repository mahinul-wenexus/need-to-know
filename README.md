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


### How to deploy something that isn't buggy?
I worked on a feature and deployed it to the production. Something is not working. And I don't know what to fix. <br>
Everything is working properly in development. But for some reason things are not working in the server.
* Why is that?

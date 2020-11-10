# Session API Reference

This reference documents all methods available in the Session API and explains in detail how these methods work.

## edit

This method creates a patch to apply changes to the session.

### Signature

The `edit` method has the following signature:

```ts
croct.session.edit(): Patch
```

The return is a patch for specifying the sequence of operations to apply to the session.
See the [patch documentation](patch.md) for more details. 

### Code Sample

Here's a minimal example showing how to edit session attributes:

```js
croct.session.edit()
  .set('plan', 'starter')
  .save()
```
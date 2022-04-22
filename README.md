# epilot-sdk

[![CI](https://github.com/epilot-dev/sdk-js/workflows/CI/badge.svg)](https://github.com/epilot-dev/sdk-js/actions?query=workflow%3ACI) [![npm version](https://img.shields.io/npm/v/epilot-sdk.svg)](https://www.npmjs.com/package/epilot-sdk) [![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/epilot-dev/sdk-js/blob/main/LICENSE)

>  ⚠️ **DISCLAIMER!**
>
> The epilot SDK is in `alpha`. Missing features, incomplete documentation and breaking API changes are to be expected!

## Quick Start

```sh
npm install --save epilot-sdk
```

```typescript
import { authenticate } from 'epilot-sdk/auth';
import entityClient from 'epilot-sdk/entity-client';

// authenticate your epilot module
const credentials = await authenticate({
  username: 'email@example.com',
  password: 'xxx',
});
credentials.configureClient(entityClient);

// use your epilot module (entity module)
await entityClient.createEntity('contact', { first_name: 'Example', last_name: 'Contact' });
```

# Documentation

- [epilot-sdk Docs](https://docs.epilot.io/docs/architecture/sdk)
- [epilot-sdk Reference](https://docs.epilot.io/api)

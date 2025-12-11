# ref-exchange-methods-const
const's for rhea/ref exchange smart contract

ℹ️ can be used with any near api js option.

---


### DEV
to devlop and publish this package
```bash
bun install
bun run index.ts
bun build index.ts
bun publish --dry-run
bunx npm login
bun publish --access public
```

---

### HOW TO USE

add
```sh
npm i @sleet-js/ref-exchange-methods-const
bun add @sleet-js/ref-exchange-methods-const
```

import
```js
import { ref_exchange_methods_const } from '@sleet-js/ref-exchange-methods-const';
```

common methods - example with near api js
```js
// GET NUMBER OF POOLS
const result = await MY_BACKEND_NEARAPI_JsonRpcProvider_const.callFunction(
  rhea_contractId_const,
  ref_exchange_methods_const.get_number_of_pools,
  {},
);

// GET SHIT BUY QUOTE
const WNEAR_IN_SHIT_OUT_RESULT = await MY_BACKEND_NEARAPI_JsonRpcProvider_const.callFunction(
  rhea_contractId_const,
  ref_exchange_methods_const.get_return,
  {"pool_id": POOLS.SHIT_WNEAR, "token_in": TOKENS.WNEAR, "amount_in": WNEAR_START_AMOUNT, "token_out": TOKENS.SHIT},
);
```

---

This project was created using `bun init` in bun v1.2.12. [Bun](https://bun.sh) is a fast all-in-one JavaScript runtime.

copyright 2025 by sleet.near
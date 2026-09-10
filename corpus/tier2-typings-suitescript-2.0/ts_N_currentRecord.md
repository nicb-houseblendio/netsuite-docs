---
id: "ts_N_currentRecord"
type: "typings"
title: "N/currentRecord (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/currentRecord"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/currentRecord.d.ts"
anchors: []
sha256: "1f4333ef8352b8cc02e277e9d5d93cce54a213fbe788660731035732bd3f7dbd"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/currentRecord.d.ts`.

```ts
import type {ClientCurrentRecord} from './record';

interface GetCurrentRecordFunction {
    (): ClientCurrentRecord;
    promise(): Promise<ClientCurrentRecord>;
}

export const get: GetCurrentRecordFunction;
```

## get

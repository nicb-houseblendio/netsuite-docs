---
id: "ts_N_config"
type: "typings"
title: "N/config (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/config"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/config.d.ts"
anchors: []
sha256: "14b14613e6070f4240028fbad5cf4fa140d621c32638dae2a428c55d105d947c"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/config.d.ts`.

```ts
import type {Record} from './record';

interface LoadOptions {
    /**
     * Use the config.Type enumeration.
     */
    type: Type;
}

/**
 * Method used to load a record.Record object that encapsulates the specified NetSuite configuration page.
 */
export declare function load(options: LoadOptions): Record;

/**
 * Enumeration that holds the string values for supported configuration pages. 
 * This enum is used to set the value of the Record.type property.
 * Note that the Record.type property is read-only.
 */
export declare enum Type {
    USER_PREFERENCES,
    COMPANY_INFORMATION,
    COMPANY_PREFERENCES,
    ACCOUNTING_PREFERENCES,
    ACCOUNTING_PERIODS,
    TAX_PERIODS,
    FEATURES,
    TIME_POST,
    TIME_VOID
}
```

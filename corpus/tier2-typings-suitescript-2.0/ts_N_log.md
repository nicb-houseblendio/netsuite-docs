---
id: "ts_N_log"
type: "typings"
title: "N/log (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/log"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/log.d.ts"
anchors: []
sha256: "9d6b71ba27bb496dcc87903949d359e2f75dac79b4447af4a1b3420c8a096e67"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/log.d.ts`.

```ts
interface LogOptions {
    /** String to appear in the Title column on the Execution Log tab of the script deployment. Maximum length is 99 characters. */
    title: string;
    /**
     * You can pass any value for this parameter.
     * If the value is a JavaScript object type, JSON.stringify(obj) is called on the object before displaying the value.
     * NetSuite truncates any resulting string over 3999 characters.
     */
    details?: any;
}

interface LogFunction {
    (title: string, details: any): void;
    (options: LogOptions): void;
}

export const debug: LogFunction;
export const audit: LogFunction;
export const error: LogFunction;
export const emergency: LogFunction;
```

## debug

## audit

## error

## emergency

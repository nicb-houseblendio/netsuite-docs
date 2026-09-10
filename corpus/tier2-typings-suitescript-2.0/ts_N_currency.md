---
id: "ts_N_currency"
type: "typings"
title: "N/currency (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/currency"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/currency.d.ts"
anchors: []
sha256: "3b60a64f9b5744af6056d0d67b3c581a90de885bd9b163ffb6a482c78b3908bd"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/currency.d.ts`.

```ts
interface ExchangeRateOptions {
    /**
     * The point in time to evaluate currency.
     */
    date?: Date;
    /**
     * The internal ID or three-letter ISO code for the currency you are converting from.
     */
    source: number | string;
    /**
     * The internal ID or three-letter ISO code for the currency you are converting to.
     */
    target: number | string;
}

/**
 * Method used to return the exchange rate between two currencies based on a certain date.
 * The exchange rate values are sourced from the Currency Exchange Rate record.
 */
export declare function exchangeRate(options: ExchangeRateOptions): number;
```

---
id: "ts_N_encode"
type: "typings"
title: "N/encode (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/encode"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/encode.d.ts"
anchors: []
sha256: "53a7208c5197837cbf02092ad5e6aed29cdb1edab48108b1e57b93895aa46902"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/encode.d.ts`.

```ts
interface ConvertOptions {
    string: string;
    inputEncoding: Encoding;
    outputEncoding: Encoding;
}

export declare enum Encoding {
    UTF_8,
    BASE_16,
    BASE_32,
    BASE_64,
    BASE_64_URL_SAFE,
    HEX,
}

/**
 * Converts a string to another type of encoding and returns the re-encoded string.
 */
export declare function convert(options: ConvertOptions): string;
```

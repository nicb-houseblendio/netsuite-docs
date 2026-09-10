---
id: "ts_N_scriptTypes_restlet"
type: "typings"
title: "N/scriptTypes/restlet (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/scriptTypes/restlet"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/scriptTypes/restlet.d.ts"
anchors: []
sha256: "d059fe62081cbde0c0d5204b3396275db06846abad8b05da3f5831b03d7536a0"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/scriptTypes/restlet.d.ts`.

```ts
/**
 * Use the N/scriptTypes/restlet module to create custom HTTP responses for your RESTlet script.
 * This module is available only to RESTlet script type.
 */

/** An HTTP response of a RESTlet script. This object is read-only. Use restlet.createResponse(options) to create and return this object. */
interface Response {
  /** The content of the RESTlet HTTP response. */
  readonly content: string;
  /** The Content-Type header of the RESTlet HTTP response. */
  readonly contentType: string;
}

/** Creates a custom RESTlet HTTP response. */
export function createResponse(options: CreateResponseOptions): Response;

interface CreateResponseOptions {
  /** The content of the response. */
  content: string;
  /**
   * The Content-Type header of the response.
   * This value overrides the default Content-Type header, which is the same as the Content-Type header of the RESTlet HTTP request.
   */
  contentType: string;
}
```

## createResponse

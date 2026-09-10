---
id: "ts_N_https_clientCertificate"
type: "typings"
title: "N/https/clientCertificate (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/https/clientCertificate"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/https/clientCertificate.d.ts"
anchors: []
sha256: "592f1f3b437c86a3e4dd61df5ee18761940546ffbba6e2dfd1ed77de46d6f49d"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/https/clientCertificate.d.ts`.

```ts
/** Load the clientCertificate module to send SSL requests with a digital certificate. */

import type {ClientResponse} from '../https';

export function post(options: { url: string, certId: string, body: string, headers?: { [key: string]: any } }): ClientResponse;
export function get(options: GetDeleteOptions): ClientResponse;
export function put(options: { url: string, certId: string, body: string, headers?: { [key: string]: any } }): ClientResponse;
declare const deleteFunc: DeleteMethod; // Workaround for the fact that "delete" is a JS keyword.
export {deleteFunc as delete};
export function request(options: RequestOptions): ClientResponse;

interface DeleteMethod {
  (options: GetDeleteOptions): ClientResponse;
}

interface GetDeleteOptions {
  /** The URL address of the remote server. */
  url: string;
  /** The ID of the client certificate. */
  certId: string;
  /** The HTTPS headers associated with the request. */
  headers?: { [key: string]: any };
}

interface RequestOptions {
  /** The URL address of the remote server. */
  url: string;
  /** The REQUEST data to be sent to the remote server. Required for PUT and POST methods | optional for HEAD, GET, DELETE. */
  body?: string;
  /** The ID of the client certificate. */
  certId: string;
  /** The HTTPS headers associated with the request. */
  headers?: { [key: string]: any };
  /** The HTTP method to be used. Use the https.Method enum to set this value. */
  method: string;
}
```

## post

## get

## put

## request

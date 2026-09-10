---
id: "ts_N_keyControl"
type: "typings"
title: "N/keyControl (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/keyControl"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/keyControl.d.ts"
anchors: []
sha256: "bf8e3bc8614802f10254f4ec578524cbb3cc791c61047fea79ec5b81784d3792"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/keyControl.d.ts`.

```ts
/**
 * The N/keyControl module can access key storage, which is also available in the UI at Setup > Company > Preferences > Keys.
 * By using the SSH keys, you can manage files and directories by using the SSH file transfer (SFTP) protocol.
 */

import type {File} from './file';

export function createKey(options: CreateKeyOptions): Key;
export function findKeys(options: FindKeysOptions): { [key: string]: any }; // TODO: Confirm return type. Documentation says its "meta-data"
export function deleteKey(options: { scriptId: string }): string; // TODO: Confirm return type. Documentation says object, but example is keyId
export function loadKey(options: { scriptId: string }): Key;

export enum Operator {
  STARTS_WITH = "startswith",
  CONTAINS = "contains",
  ENDS_WITH = "endswith",
  EQUALS = "equals"
}

interface Key {
  file: File;
  /** The password of the key. GUID or secret token for working with passwords is accepted. */
  password: string;
  /** The script ID of the key. Using Key.save() and keyControl.findKeys(options) returns the script ID. */
  scriptId: string;
  name: string;
  description: string;
  /** An array of employee IDs. Only these employees can access the key. */
  restrictions: string[];
  save: () => void; // TODO: Verify return type. Documentation says it returns an object?
}

interface CreateKeyOptions {
  file?: File;
  /** The password of the key. GUID or secret token for working with passwords is accepted. */
  password?: string;
  /** The script ID of the key. Using Key.save() and keyControl.findKeys(options) returns the script ID. */
  scriptId?: string;
  name?: string;
  description?: string;
  /** An array of employee IDs. Only these employees can access the key. */
  restrictions?: string[]|number[];
}

interface FindKeysOptions {
  /**
   * The name of the key.
   * The properties of the object are:
   * - value is a string, which can be used if object is used instead of string.
   * - operator is one of the operator enum.
   * - ignoreCase is either true or false.
   * If the object is used, the value is mandatory. Operator defaults to equals and ignoreCase defaults to true.
   */
  name?: string|{ value: string, operator?: string, ignoreCase?: boolean };
  description?: string;
  /** The internal ID of an employee selected in the Restrict to Employees field. */
  restriction?: number;
}
```

## createKey

## findKeys

## deleteKey

## loadKey

## Operator

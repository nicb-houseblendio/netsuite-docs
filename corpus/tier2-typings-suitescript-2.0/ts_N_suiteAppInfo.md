---
id: "ts_N_suiteAppInfo"
type: "typings"
title: "N/suiteAppInfo (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/suiteAppInfo"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/suiteAppInfo.d.ts"
anchors: []
sha256: "8c3b3af9f05c1c94e0770f79361cdfb7e10369eecb54e447a7aea2db7a692f6b"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/suiteAppInfo.d.ts`.

```ts
/**
 * Load the N/suiteAppInfo module when you want to access information related to SuiteApps and Bundles.
 * This module is available for all script types.
 */

export function isBundleInstalled(options: { bundleId: number|string }): boolean;
export function isSuiteAppInstalled(options: { suiteAppId: string }): boolean;

/** This method returns the IDs for bundles that contain the specified script, for each individual script specified. */
export function listBundlesContainingScripts(options: { scriptIds: string[] }): { [scriptId: string]: number[] };

/** This method returns a list of successfully installed bundles, as an array of objects. */
export function listInstalledBundles(): IBundle[];

export function listInstalledSuiteApps(): ISuiteApp[];

/**
 * Returns the ID for the SDF SuiteApp that contains the specified script, for each individual script specified.
 * Only one ID will be returned for each specified script.
 */
export function listSuiteAppsContainingScripts(options: { scriptIds: string[] }): { [scriptId: string]: string };

interface IBundle {
  id: number;
  name: string;
  version: string;
  description: string;
  installedFrom: string;
  isManaged: boolean;
  dateInstalled: Date;
  dateLastUpdated: Date;
  publisher:   { id: string; name: string };
  installedBy: { id: number; name: string };
}

interface ISuiteApp {
  appId: string;
  name: string;
  version: string;
  description: string;
  dateInstalled: Date;
  dateLastUpdated: Date;
  publisherId: string;
  installedBy: { id: number; name: string };
}
```

## isBundleInstalled

## isSuiteAppInstalled

## listBundlesContainingScripts

## listInstalledBundles

## listInstalledSuiteApps

## listSuiteAppsContainingScripts

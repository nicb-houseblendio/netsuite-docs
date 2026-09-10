---
id: "ts_N_commerce_recordView"
type: "typings"
title: "N/commerce/recordView (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/commerce/recordView"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/commerce/recordView.d.ts"
anchors: []
sha256: "60475fe5fa75a49a844a6ae545fb4aa6cfdf8f32367211d0317c9556e5d189ec"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/commerce/recordView.d.ts`.

```ts
/** Load the N/commerce/recordView module when you want to provide fast, cached, and public access to the item fields and website settings. */

/** Retrieves one or more Items with requested items fields from an Item Record. */
export declare function viewItems(): { [fieldId: string]: string|number|boolean };

/** Retrieves the website details with requested website fields. */
export declare function viewWebsite(): { [fieldId: string]: string|number|boolean };

interface RecordViewOptions {
  /** IDs of the item you want to view */
  ids: number[];
  /** Item fields you want to retrieve for the items */
  fields: string|string[];
  /**
   * Options that affect related fields. Array of name, value pairs. Type depends upon parameter.
   * Supported field options (viewItems only):
   * - includeVat: this affects onlinecustomerprice_detail field. Default value is false.
   */
  fieldOptions?: { [fieldId: string]: string|boolean }[];
}
```

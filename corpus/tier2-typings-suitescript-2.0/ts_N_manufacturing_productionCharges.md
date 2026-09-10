---
id: "ts_N_manufacturing_productionCharges"
type: "typings"
title: "N/manufacturing/productionCharges (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/manufacturing/productionCharges"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/manufacturing/productionCharges.d.ts"
anchors: []
sha256: "231c69baa5b3a1db5bfd8871feeef42c54a4596d6ed42ffeb807ef29c035f931"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/manufacturing/productionCharges.d.ts`.

```ts
/**
 * Use the N/manufacturing/productionCharges module to update unit costs of manufacturing charges
 * on Assembly Build, Work Order Close, and Work Order Completion transactions.
 *
 * Prerequisites: the Assembly Items feature and the "Allow bulk cost updates for Production Charges"
 * preference must be enabled, and the user needs at least Edit permission on the relevant transactions.
 * Transactions modified by this module must be of type Assembly Build, Work Order Completion, or
 * Work Order Issue, and must be in an open posting period.
 *
 * Note: This module is only usable in server-side SuiteScript 2.1 scripts.
 * Note: Cost changes made using this module do not trigger other SuiteScript scripts.
 * @since 2026.1
 */

/**
 * Updates cost on specific transaction lines to a specified unit cost.
 *
 * Applies to transaction lines that are credit lines (quantity less than 0), are of type
 * Non-Inventory, Service, or Other Charge, use items designated for Purchase or Resale, and use
 * items whose cost category is not of type Outsourcing Charge, Landed, or Service.
 * @governance none
 */
export function updateChargesToCustomUnitCost(options: {
    /** ID of transaction to be updated. */
    transactionId: number,
    /** Array of IDs of lines to be updated. */
    transactionLineIds: number[],
    /** New unit cost of item on transaction line. */
    newUnitCost: number,
    /**
     * Default value is true. When true, for lines with the Multiple Units of Measure feature enabled,
     * the new unit cost is applied as the unit cost of the base unit. When false, it is applied as a
     * fixed unit cost value irrespective of any Multiple Units of Measure conversion rates.
     * This parameter can only be used when the Multiple Units of Measure feature is enabled.
     */
    isUnitCostPerBaseUnit?: boolean,
}): void;

/**
 * Updates cost on specific transaction lines according to the current purchase price of the originating item.
 *
 * Applies to the same transaction line criteria as updateChargesToCustomUnitCost.
 * @governance none
 */
export function updateChargesToItemPurchasePrice(options: {
    /** ID of transaction to be updated. */
    transactionId: number,
    /** Array of IDs of lines to be updated. */
    transactionLineIds: number[],
}): void;

/**
 * Updates cost on all routing and non-inventory transaction lines on a specified transaction to the current price.
 * @governance none
 */
export function updateAllChargesToItemPurchasePrice(options: {
    /** ID of transaction to be updated. */
    transactionId: number,
}): void;
```

## updateChargesToCustomUnitCost

## updateChargesToItemPurchasePrice

## updateAllChargesToItemPurchasePrice

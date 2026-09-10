---
id: "ts_N_util"
type: "typings"
title: "N/util (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/util"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/util.d.ts"
anchors: []
sha256: "b3303b7e490d144d05b566930613a3fe0c19be690f29d3527301951da7c0ada1"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/util.d.ts`.

```ts
export function isArray(obj: any): obj is any[];
export function isBoolean(obj: any): obj is boolean;
export function isDate(obj: any): obj is Date;
export function isNumber(obj: any): obj is number;
export function isObject(obj: any): obj is object;
export function isRegExp(obj: any): obj is RegExp;
export function isString(obj: any): obj is string;
export function isFunction(obj: any): obj is Function;

/**
 * Returns the number of nanoseconds elapsed since an arbitrary epoch.
 * Use this to calculate the time between two events.
 */
export function nanoTime(): number;

/**
 * Iterate over each element of an array or each property of an object.
 * @param iterable
 * @param callback
 */
export function each<T>(iterable: T[], callback: (item: T, idx: number, iterable: T[]) => void): T[];
export function each<T>(iterable: T, callback: (property: any, key: keyof T, iterable: T) => void): T;

/**
 * Copy all properties from contributor into receiver.
 * Properties in contributor that are already in receiver get overwritten.
 * @param receiver
 * @param contributor
 */
export function extend<T, U>(receiver: T, contributor: U): T & U;
```

## isArray

## isBoolean

## isDate

## isNumber

## isObject

## isRegExp

## isString

## isFunction

## nanoTime

## each

## extend

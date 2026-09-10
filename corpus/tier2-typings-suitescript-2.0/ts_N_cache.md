---
id: "ts_N_cache"
type: "typings"
title: "N/cache (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/cache"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/cache.d.ts"
anchors: []
sha256: "4cb9ed01fe7328d35760c2afbf492704a8525cc31d0c91cb2752bf3b69621681"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/cache.d.ts`.

```ts
interface LoaderContext {
    key: string;
}

interface GetOptions {
    /** A string that identifies the value to be retrieved from the cache. This value cannot be null. */
    key: string;

    /**
     * Optional, but strongly recommended
     * A user-defined function that returns the requested value if it is not already present in the cache. Additionally, when the loader retrieves a value, the system automatically places that value in the cache. For this reason, NetSuite recommends using the loader function as the primary means of populating the cache.
     * Note also that if the value returned by the loader is not a string, the system uses JSON.stringify() to convert the value before it is placed in the cache and returned. The maximum size of a value that can be placed in the cache is 500KB.
     * When no loader is specified and a value is missing from the cache, the system returns null.
     */
    loader?: (context: LoaderContext) => string;

    /** The duration, in seconds, that a value retrieved by the loader should remain in the cache. The default time to live, or TTL, is no limit. The minimum value is 300 (five minutes). */
    ttl?: number;
}

interface PutOptions {
    /** An identifier of the value that is being cached. The maximum size of the cache key is 4 kilobytes. */
    key: string;

    /** The value to place in the cache. If the value submitted is not a string, the system uses JSON.stringify() to convert the value before it is placed in the cache. The maximum size of the value is 500KB. */
    value: string;

    /** The duration, in seconds, that a value retrieved by the loader should remain in the cache. The default time to live, or TTL, is no limit. The minimum value is 300 (five minutes). */
    ttl?: number;
}

interface RemoveOptions {
    /** An identifier of the value that is being removed. */
    key: string;
}

export interface Cache {
    /** A label that identifies the cache. */
    name: string;

    /** A value that describes the availability of the cache. A cache can be made available to the current script only, to all scripts in the current bundle, or to all scripts in your NetSuite account. */
    scope: string | Scope;

    /** Retrieves a value from the cache based on a key that you provide. If the requested value is not present in the cache, the method uses the user-defined function identified by the method’s option.loader parameter. The value retrieved by this function is cached and then returned. */
    get(options: GetOptions): string | null;

    /** Puts a value into the cache. If the value provided is not a string, the system uses JSON.stringify() to convert the value to a string. */
    put(options: PutOptions): void;

    /** Removes a value from the cache. */
    remove(options: RemoveOptions): void;
}

interface GetCacheOptions {
    /** A label that will identify the cache you are creating. The maximum size of the cache name is 1 kilobyte. */
    name: string;

    /** The scope of the cache. This value determines the availability of the cache. A cache can be made available to the current script only, to all scripts in the current bundle, or to all scripts in your NetSuite account. */
    scope?: Scope;
}

/** Checks for a cache object with the specified name. If the cache exists, this method returns the cache object. If the cache does not exist, the system creates it. */
export function getCache(options: GetCacheOptions): Cache;

export enum Scope {
    /** The cache is available only to the current script. This value is the default. */
    PRIVATE,

    /**
     * The cache is available only to some scripts, as follows:
     *  - If the script is part of a bundle, the cache is available to all scripts in the same bundle.
     *  - If the script is not in a bundle, then the cache is available to all scripts not in a bundle.
     */
    PROTECTED,

    /** The cache is available to any script in the NetSuite account. */
    PUBLIC,
}
```

## Cache

## getCache

## Scope

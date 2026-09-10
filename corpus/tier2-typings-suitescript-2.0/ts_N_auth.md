---
id: "ts_N_auth"
type: "typings"
title: "N/auth (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/auth"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/auth.d.ts"
anchors: []
sha256: "88652bbef73ab00c38ab0deb206b5ab6411db62b8f7118f1eb4cc89a33a0f063"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/auth.d.ts`.

```ts
interface ChangePasswordOptions {
    currentPassword: string;
    newPassword: string;
}

interface ChangeEmailOptions {
    password: string;
    newEmail: string;
    onlyThisAccount?: boolean;
}

/**
 * Method used to change the current user’s NetSuite email address (user name).
 */
export declare function changeEmail(options: ChangeEmailOptions): void;

/**
 * Method used to change the current user’s NetSuite password.
 */
export declare function changePassword(options: ChangePasswordOptions): void;
```

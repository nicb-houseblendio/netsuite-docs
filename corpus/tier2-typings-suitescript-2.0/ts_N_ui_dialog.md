---
id: "ts_N_ui_dialog"
type: "typings"
title: "N/ui/dialog (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/ui/dialog"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/ui/dialog.d.ts"
anchors: []
sha256: "c3a4e412e9df4afd38d84f1aa1c3b827468092c394992de3b776d50590501a29"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/ui/dialog.d.ts`.

```ts

interface AlertOptions {
    title?: string;
    message?: string;
}

interface CreateDialogOptions {
    buttons?: DialogButton[];
    title?: string;
    message?: string;
}

interface DialogButton {
    label: string;
    value: number | string;
}

export function alert(options: AlertOptions): Promise<boolean>;
export function confirm(options: AlertOptions): Promise<boolean>;
export function create(options: CreateDialogOptions): Promise<string>;
```

## alert

## confirm

## create

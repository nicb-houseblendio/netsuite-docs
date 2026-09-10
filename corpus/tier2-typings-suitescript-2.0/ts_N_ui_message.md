---
id: "ts_N_ui_message"
type: "typings"
title: "N/ui/message (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/ui/message"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/ui/message.d.ts"
anchors: []
sha256: "11d23201e73b1f23ede3307ba5d3d2986293b35c4acc4eab181b0d997da5ff34"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/ui/message.d.ts`.

```ts
export interface Message { // Also referenced in N/ui/serverWidget
    hide(): void;
    show(options?: MessageShowOptions): void;
}

export interface MessageCreateOptions {
    message?: string;
    title?: string;
    type: Type;
    /**
     * The amount of time, in milliseconds, to show the message. The default is 0, which shows the message until Message.hide() is called.
     * If you specify a duration for message.create() and message.show(), the value from the message.show() method call takes precedence.
     */
    duration?: number;
}

interface MessageShowOptions {
    duration?: number;
}

export function create(options: MessageCreateOptions): Message;
export enum Type {
    CONFIRMATION, // A green background with a checkmark icon.
    INFORMATION,  // A blue background with an Information icon.
    WARNING,      // A yellow background with a Warning icon.
    ERROR,        // A red background with an X icon.
}
```

## Message

## MessageCreateOptions

## create

## Type

---
id: "ts_N_workflow"
type: "typings"
title: "N/workflow (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > N/workflow"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/N/workflow.d.ts"
anchors: []
sha256: "b6d0e343a553682f817448733f3f673c215ae3332312c1d6b9183c0c1eb95840"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `N/workflow.d.ts`.

```ts
import type {Type} from "./record";

interface InitiateOptions {
    recordType: string | Type;
    recordId: string | number;
    workflowId: string | number;
    defaultValues?: any;
}

interface TriggerOptions {
    recordType: string | Type;
    recordId: string | number;
    /**
     * Internal ID (number) or script ID (string) for the workflow definition. This is the ID field on the Workflow Definition Page.
     */
    workflowId: string | number;
    workflowInstanceId?: number | string;
    defaultValues?: any;
    /**
     * Internal ID of a button that appears on the record in the workflow.
     * Use this parameter to trigger the workflow as if the specified button were clicked.
     */
    actionId?: string | number;
    /** The internal ID (number) or script ID (string) of the workflow state that contains the action. */
    stateId?: string | number;
}

export function initiate(options: InitiateOptions): number;
export function trigger(options: TriggerOptions): number;
```

## initiate

## trigger

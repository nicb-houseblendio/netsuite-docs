---
id: "ts_EmailCapturePlugin"
type: "typings"
title: "EmailCapturePlugin (SuiteScript 2.x typings)"
branch: "tier2-typings-suitescript-2.0"
category: "tier2"
breadcrumb: "SuiteScript 2.x Typings > EmailCapturePlugin"
parent: null
source: "https://github.com/headintheclouddev/typings-suitescript-2.0/blob/b84ad47f78e50f18c07420b44634562d8c972e01/EmailCapturePlugin.d.ts"
anchors: []
sha256: "6d16ac5a4168d10b5fbe6e90b68dd4fba45f5b177b30f6c545d8f561b56d37f7"
---

SuiteScript 2.x community typings (MIT) — [headintheclouddev/typings-suitescript-2.0](https://github.com/headintheclouddev/typings-suitescript-2.0)@b84ad47 — `EmailCapturePlugin.d.ts`.

```ts
interface IAddress {
  getEmail(): string;
  getName():  string;
}

interface IAttachment {
  /**
   * Object that represents an attachment in an email message sent to an Email Capture plug-in implementation.
   * Each Attachment object contains properties for the attachment file name, attachment type, and the value of the attachment file.
   */
  getName(): string;
  /** Returns the file type of an attachment in an email message as a string. For example, this method returns PLAINTEXT, PDF, and MISCBINARY for text, PDF, and Microsoft Word files, respectively. */
  getType(): string;
  /**
   * Returns a text string for a text file attachment or base-64 encoded string for binary attachment types of an email message.
   * You can use getType() to define the behavior of the plug-in implementation depending on the file type of the attachment.
   */
  getValue(): string;
}

/** Object that represents an email message sent to the Email Capture plug-in implementation. */
interface IEmail {
  getAttachments(): IAttachment[];
  getCc():          IAddress[];
  getFrom():        IAddress; // Documentation incorrectly shows this as an array, but an email only comes from one address.
  getHtmlBody():    string;
  getReplyTo():     IAddress;
  getSentDate():    Date;
  getSubject():     string;
  getTextBody():    string;
  getTo():          IAddress[]; // Documentation incorrectly shows this as a single address, but testing confirms that it's an array.
}
```

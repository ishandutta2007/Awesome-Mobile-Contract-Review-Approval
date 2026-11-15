# Awesome-Mobile-Contract-Review-Approval

# Awesome Mobile Contract Review & Approval

> A curated list of top Mobile Contract Review and Approval platforms — both SaaS/Hosted commercial solutions and open-source alternatives for reviewing, redlining, and approving contracts from mobile devices.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Docusign Mobile](#docusign-mobile)
  - [Adobe Acrobat Sign Mobile](#adobe-acrobat-sign-mobile)
  - [PandaDoc Mobile](#pandadoc-mobile)
  - [Ironclad](#ironclad)
  - [Conga Contracts Mobile](#conga-contracts-mobile)
  - [SignNow Mobile](#signnow-mobile)
  - [Coupa Mobile Approvals](#coupa-mobile-approvals)
- [Open-Source Software](#-open-source-software)
  - [draftLegal](#draftlegal)
  - [OpenCLM](#openclm)
  - [DocuSeal](#docuseal)
  - [Click2Approve](#click2approve)
  - [OnlyOffice Documents](#onlyoffice-documents)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Mobile Contract Review and Approval platforms. These are not open-source but are included as reference points for feature comparison.

### Docusign Mobile
**Type:** Mobile e-signature and agreement management
Docusign's redesigned mobile app allows users to upload documents by scanning with the camera or importing from cloud storage, tag signature fields with drag-and-drop, and send for signature via email or Google Drive [citation:2]. Real-time push notifications alert users when a document is signed, and reminders can be sent with a single tap [citation:11]. The app includes a dashboard showing pending, completed, and waiting agreements, with the ability to manage the entire workflow from a phone or tablet [citation:2]. **Note:** The app focuses on e-signature and status tracking rather than deep contract redlining or clause-level review on mobile.

### Adobe Acrobat Sign Mobile
**Type:** Mobile e-signature with offline support
Adobe Acrobat Sign provides a mobile companion for its e-signature service, allowing users to open and sign documents instantly, read them in Reading Mode before signing, and sign directly on screen with a finger or stylus [citation:3]. A key differentiator is **offline signing**—documents can be signed without connectivity and sync automatically when back online [citation:3]. It supports delegating signing to another person or rejecting requests, saving partially filled forms, and sending documents for signature from cloud storage like Google Drive, Box, or Dropbox [citation:3]. Signed documents are saved as Certified PDFs with a complete audit trail and signer geolocation can be added [citation:3]. **Trade-off:** The app is e-signature focused; contract review and redlining happen in the broader Adobe Acrobat ecosystem rather than the mobile app itself.

### PandaDoc Mobile
**Type:** Mobile document creation and approval
PandaDoc's mobile app allows users to create documents from scratch or from templates, send them, and collect e-signatures [citation:12]. It provides **real-time alerts** when someone opens, views, or completes a document, and supports viewing any document, approving it for signature, and managing the inbox directly from the phone [citation:12]. Comments and responses can be handled through the app, and reminders can be sent to recipients [citation:12]. **Trade-off:** Mobile approval is supported, but the deeper redlining and workflow configuration capabilities remain in the desktop/web version.

### Ironclad
**Type:** Contract workflow with mobile signing
Ironclad's platform includes mobile lease signing, with the company reporting a **3x increase in mobile lease signing** [citation:13]. The workflow includes a Launch Form for intake, a Review step where internal Approvers approve each version, and a Share Document step that sends the contract to the counterparty via email (they do not need to log into Ironclad) [citation:5]. The Activity Feed records internal collaboration and @mentions [citation:5]. **Trade-off:** Ironclad's mobile experience is focused on signing and notifications rather than full contract review or redlining on the device.

### Conga Contracts Mobile
**Type:** Slim mobile interface for contract approvals
Conga Contracts provides a **Slim Mobile Interface** accessible from iOS, BlackBerry, or Android devices, allowing users to view company and contract information and perform tasks like downloading documents, closing events, completing tasks, and **approving or declining Gateway steps in a workflow** [citation:6]. The interface is web-based (navigate to the contracts URL on a mobile browser) rather than a native app, and is designed for basic approval actions rather than document editing.

### SignNow Mobile
**Type:** Mobile e-signature with kiosk mode
SignNow provides mobile e-signing with offline mode, the ability to sign documents digitally, fill and complete PDF/Word/rich text documents, and send signature requests to multiple recipients [citation:7]. It includes **Kiosk Mode** for events and waiting rooms, where a new document is generated for each signer while hiding other documents [citation:7]. It supports capturing photo IDs for signature verification, a detailed audit history, and team document sharing. **Trade-off:** Focused on signing and form completion rather than contract review workflows.

### Coupa Mobile Approvals
**Type:** Mobile procurement and contract approvals
Coupa provides mobile approvals for procurement requisitions and contract-related spend, allowing users to check the status of purchasing requisitions and approve or reject items from anywhere on any device [citation:8]. The platform's central contract repository surfaces preferred supplier contracts at the top of search results, and guided buying steers users to contracted items [citation:8]. **Trade-off:** Mobile functionality is focused on approval actions within the procurement workflow rather than contract review or redlining.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Mobile Contract Review and Approval tools. The open-source ecosystem spans **AI-native CLM with mobile-accessible workflows**, **full contract lifecycle platforms**, **e-signature platforms with mobile-optimized UIs**, and **document approval systems**.

### draftLegal
**Stack:** TypeScript / Python / Docker | **License:** AGPL-3.0
draftLegal is explicitly positioned as **"the open-source alternative to Ironclad + Harvey"** — a self-hosted, AI-native contract lifecycle management platform where contracts never leave your servers [citation:16]. For review and approval, it provides **agent-first workflows** with ~30 tools over contracts including search, cite, compare, draft, redline, and route approvals, with every write proposed on a confirm card first and most actions undoable [citation:16]. **Redline & negotiate** capabilities offer conservative/moderate/aggressive counter-proposals with exact replacement language [citation:16]. **Full lifecycle** coverage includes approval workflows, in-platform e-signature, and post-signature obligation tracking [citation:16]. The platform is **web-based and accessible from mobile browsers**, though there is no dedicated native mobile app. **Important:** Early-stage project; review repository status before production use.

### OpenCLM
**Stack:** TypeScript / PostgreSQL / Docker | **License:** AGPL-3.0
OpenCLM is an open-source, self-hostable contract lifecycle management platform with **collaborative redlining, review workflows, electronic signatures, sealed PDFs, and API-first integrations** [citation:15][citation:21]. Key features include a contract repository, clause and template management, approval workflows, deadlines, obligations, analytics, and role-based access control [citation:21]. Executed PDFs carry document-native signatures, an embedded completion record, and a PAdES-B-B detached CMS platform seal with a public verification page [citation:15]. **Important status:** The README states this is an **early development release**, and the signature is an ordinary electronic signature (not advanced or qualified) with no long-term-validation material [citation:15]. Access is via web interface, which is responsive and usable on mobile browsers.

### DocuSeal
**Stack:** Ruby / PostgreSQL | **License:** AGPL-3.0
DocuSeal is an open-source document signing platform with a **mobile-optimized UI** and a native iOS app (available on the App Store) [citation:19][citation:29]. It supports creating PDF forms, sending them for signature, tracking who has signed, and scanning paper documents into templates [citation:19]. Features include WYSIWYG PDF forms, 12 field types, multi-signer support, SMTP auto emails, S3/GCS/Azure storage, eSign and verify, API and webhooks [citation:29]. It has approximately **10.5k GitHub stars** [citation:29]. **Trade-off:** DocuSeal is focused on the **signing** layer rather than contract review, redlining, or approval workflows—it is the e-signature component that could complement a review platform.

### Click2Approve
**Stack:** .NET / SQL Server / Docker | **License:** MIT
Click2Approve is an open-source document approval and workflow system that supports **document approval workflows with multi-step sequential or parallel assignees**, flexible task actions (approval, signature, confirmation, review, acceptance), and electronic signatures with IP address and browser evidence [citation:22]. It includes file uploads and previews, request and task tracking, email and in-app notifications, and a **responsive web interface** that can be managed from desktop or mobile [citation:22]. It is MIT-licensed, making it permissive for commercial use. **Trade-off:** It is a general document approval platform rather than a contract-specific CLM—it lacks contract clause management, redlining, or obligation tracking.

### OnlyOffice Documents
**Stack:** Native mobile apps (Android/iOS) | **License:** AGPL-3.0 (Community)
OnlyOffice Documents provides native mobile apps for Android and iOS with **track changes and review functionality** [citation:28][citation:18]. The Reviews panel allows users to activate Track Changes mode, choose display modes (Markup, Final, Original), navigate between changes, and accept or reject individual changes or all changes at once [citation:18]. Document access permissions include a **Review** mode where changes need approval [citation:28]. While not a contract management platform, it provides the core **redlining and review capability** on mobile that a contract workflow requires—it could serve as the document editing layer alongside an approval system.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Mobile Access | Review/Redline | E-Signature | Self-Hosted | Best For |
|----------|---------|-------|---------------|----------------|-------------|-------------|----------|
| **Docusign** | Proprietary | Cloud | ✅ Native | (Limited) | ✅ | ❌ | Mobile e-signature standard |
| **Adobe Acrobat Sign** | Proprietary | Cloud | ✅ Native | (Reading Mode) | ✅ Offline | ❌ | Offline signing + audit |
| **PandaDoc** | Proprietary | Cloud | ✅ Native | (Approval) | ✅ | ❌ | Mobile document approval |
| **Ironclad** | Proprietary | Cloud | ✅ (Signing) | (Desktop) | ✅ | ❌ | Workflow + mobile signing |
| **Conga Contracts** | Proprietary | Cloud | ✅ Web (Slim) | ❌ | (Check) | ❌ | Basic mobile approvals |
| **draftLegal** | AGPL-3.0 | TypeScript/Docker | ✅ Web | ✅ AI redline | ✅ | ✅ | Self-hosted AI CLM + redline |
| **OpenCLM** | AGPL-3.0 | TypeScript/Postgres | ✅ Web | ✅ Redlining | ✅ PAdES | ✅ | Self-hosted full CLM |
| **DocuSeal** | AGPL-3.0 | Ruby/Postgres | ✅ Native iOS | ❌ (Signing) | ✅ | ✅ | Open-source e-signature |
| **Click2Approve** | MIT | .NET/SQL | ✅ Responsive | ❌ (Approval) | ✅ | ✅ | Document approval workflows |
| **OnlyOffice** | AGPL-3.0 | Native apps | ✅ Native | ✅ Track changes | ❌ | ✅ (DocSpace) | Mobile document redlining |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Mobile Contract Review or Approval tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The open-source landscape for **mobile contract review and approval** is **fragmented across layers** rather than unified platforms. **draftLegal** and **OpenCLM** provide full contract lifecycle management with AI-assisted redlining and approval workflows, accessible via mobile browsers, though both are early-stage [citation:15][citation:16]. **DocuSeal** fills the e-signature layer with a native iOS app [citation:19]. **OnlyOffice** provides the mobile redlining and track-changes capability that a contract workflow requires [citation:18]. **Click2Approve** offers a permissive MIT-licensed approval workflow foundation [citation:22]. No single open-source project replicates Ironclad's breadth of intake-to-signature workflow with a polished mobile experience, but combinations of these tools can cover the core review, approval, and signing workflow for self-hosted deployments.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐

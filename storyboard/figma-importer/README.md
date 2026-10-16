# English comparison panel — Figma local importer

[中文总目录](../README.md) · [独立中文 PDF 说明](../downloads/chinese-explanation.pdf) · [下载完整导入源码与数据 ZIP](../downloads/figma-import-package.zip)

**The panel has NOT been added to the user's Figma file from this environment.** Figma access is blocked here, and no live Figma editing tool is available. This package prepares the complete English content and a local importer that can run in the user's authorized Figma session.

## Intended result

- A new panel named **Website vs. Design Storyboard Comparison** below existing content on the page named **Brain storm**.
- 153 website evidence captures in order, with English action, observed result, limitations and uncertainty labels.
- Local previews from existing source frames, components and instances on Brain storm, plus the two supplied reference-node subtrees when accessible.
- Every name-matched candidate is retained and marked **tentative**. Unmatched sources remain in the gallery. The importer never treats a name match as a confirmed design comparison.
- Existing source content is preserved. A repeated import stops if the comparison panel already exists.

## Run in Figma Desktop

1. Download and extract `figma-import-package.zip` from the link above.
2. Open the supplied Figma Design file in Figma Desktop. Verify the file and the **Brain storm** page yourself; local plugins may be unable to read a file key.
3. Use **Plugins → Development → New plugin**, choose **Figma Design** and **Custom UI**, and save the generated local plugin folder. Figma assigns the plugin ID; this repository does not fabricate one.
4. Replace the generated `code.js` and `ui.html` with the supplied files. Keep Figma's generated `id` in its manifest. Use `manifest.template.json` for the remaining fields: `main`, `ui`, `documentAccess: dynamic-page`, and `networkAccess.allowedDomains: ["none"]`.
5. Run that development plugin. In its UI select **all 25 JSON chapter files** from the package's `payloads` folder. Confirm that it reports **153 scenes**.
6. Choose **Import at the bottom of Brain storm**. Keep Figma open while evidence and the local source gallery are added. Large source pages can take time; source previews are exported within the current session.
7. Review the new panel. All automatic design matches remain uncertain. If the page is absent/ambiguous or the panel already exists, the importer stops rather than guessing or overwriting.

If “Brain storm” is actually a section/frame rather than a Figma **page**, this version deliberately stops. It does not guess a container or resize existing content. A real file inspection is needed to adapt that target safely.

## What was checked

- JavaScript syntax and local mock-API integration checks passed for sequence handling, retaining multiple candidates, absent/duplicate target protection, placement below existing bounds, completion labels and preservation of the original node.
- All 153 English records and screenshots are included across 25 chapter files. The package uses local file inputs and the Figma session; the plugin declares no network destinations.
- API usage was reviewed against Figma's published plugin typings.
- **Not checked in a live Figma file:** manifest registration, the actual Brain storm page/container, source-frame candidates, rendering limits, client performance or the final appearance. This is an import package, not evidence of a completed import.

## Content limits

Website capture date: 2026-10-16. Signed-in website features and the 3D exhibition interior were not verified. The main site's Google login fails with `401 deleted_client`; the independent 3D Google entry reaches a normal sign-in page. Seven native players have playback-start evidence; two embedded players remain unconfirmed.

Screenshots retain the original website language. Newly created annotations and panel labels are English. Original source-frame names and design text are preserved rather than rewritten.

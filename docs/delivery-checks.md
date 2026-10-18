# Delivery checks and project boundary

This repository is a single HTML demand-planning prototype. Its page explicitly labels the data as sample/anonymized and says nothing here is live. Preserve that boundary.

This is structural verification, not proof of calendar behavior, pricing, capacity rules or live booking correctness. A change to prototype behavior also needs focused interaction verification against its sample data. Do not connect this prototype to customer systems or provision a deployment merely to finish this governance change.

There is no established Git-linked Vercel target in the inspected team inventory. Record source/check evidence for governance completion. Deployment requires an actual authorized product outcome and a verified target.

Follow [SOFTWARE_DELIVERY.md](../SOFTWARE_DELIVERY.md) and the adapted skill for proportional brainstorming, planning, independent final-diff review and authorized delivery.

## Enumerated source verification

- Supported local resources (tracked paths): script/img/source/video/audio/iframe src; video poster; link href for ASCII-case-insensitive stylesheet/icon/preload/modulepreload; img/source srcset; CSS url(...) and quoted @import in lowercase .css, style blocks and style attributes.

- Supported anchors: #id and explicit local .html#id targets and IDs. Supported syntax: inline classic/module scripts, lowercase .js/.mjs sources and their local static import/re-export graph, and FunctionBody syntax for the finite handler list below. Script/style EOF and repository path escapes are rejected; any base[href] is unsupported and fails closed.

- Handler allowlist (HTML GlobalEventHandlers snapshot, not all DOM handlers): onabort onauxclick onbeforeinput onbeforematch onbeforetoggle onblur oncancel oncanplay oncanplaythrough onchange onclick onclose oncommand oncontextlost oncontextmenu oncontextrestored oncopy oncuechange oncut ondblclick ondrag ondragend ondragenter ondragleave ondragover ondragstart ondrop ondurationchange onemptied onended onerror onfocus onformdata oninput oninvalid onkeydown onkeypress onkeyup onload onloadeddata onloadedmetadata onloadstart onmousedown onmouseenter onmouseleave onmousemove onmouseout onmouseover onmouseup onpaste onpause onplay onplaying onprogress onratechange onreset onresize onscroll onscrollend onsecuritypolicyviolation onseeked onseeking onselect onslotchange onstalled onsubmit onsuspend ontimeupdate ontoggle onvolumechange onwaiting onwebkitanimationend onwebkitanimationiteration onwebkitanimationstart onwebkittransitionend onwheel

- Unverified extensions: query-only same-page fragments; manifest links; track/object/embed/image-input resource attributes; CSS image-set string candidates; nonlowercase/extensionless or other local script/dependency filenames; other event-handler families; bare/import-map/dynamic module resolution; plain navigation and rewritten routes.

- Limits: lowercase .html/.css/.js/.mjs source loading only; bounded lexical CSS/HTML checks, not full parser/error recovery, module linking/evaluation, image selection/fetch, DOM execution or production/user-flow proof. Use focused verification or a scoped extension for an outcome relying on an unverified surface.

The checker prints this same contract in `--help` and after successful supported checks. An `UNVERIFIED` diagnostic identifies an observed surface outside that contract; it is not a syntax/resource pass for that surface. Ordinary unfamiliar attributes such as `onboarding` are inert data and are not rejected as handlers. The finite handler list is sourced from the [HTML GlobalEventHandlers IDL snapshot](https://html.spec.whatwg.org/multipage/webappapis.html#handler-globaleventhandlers), October 18, 2026; other standards and Window-only handlers are not claimed.

A changed outcome relying on an unverified extension needs focused verification or a separately scoped checker improvement. This does not require Todd to choose engineering tactics. No new dependency, universal unknown-HTML ban, full browser validator or production behavior claim is introduced.

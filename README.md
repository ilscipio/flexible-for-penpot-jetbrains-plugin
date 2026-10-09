![Rating](https://img.shields.io/jetbrains/plugin/r/stars/34826) ![Downloads](https://img.shields.io/jetbrains/plugin/d/34826) ![Version](https://img.shields.io/jetbrains/plugin/v/34826)

<img src="logo.png" alt="Flexible for Penpot" width="96">

# [Flexible for Penpot](https://plugins.jetbrains.com/plugin/34826-flexible-for-penpot)
Your Penpot design system in JetBrains IDEs: components with their variants, valid combinations and tokens, CSS
generated from the design, links from your component files to Penpot with notices when the design changes, and Penpot
design tokens in CSS, SCSS and Less with completion, hover and inspections. A generated stylesheet holds all tokens and
themes, also as a Tailwind CSS v4 theme and as TypeScript. Works with design.penpot.app and with your own Penpot server.

**Flexible for Penpot is a young plugin. Please leave a review, open a GitHub issue, or write to info@ilscipio.com. Report a
bug or an idea and get 20% off the annual license, or one month free.**

## Core Features

### Components and Variants
* **Components** of your Penpot library with folders, variant sets, a preview and a link to the component in Penpot
* **Variant pickers**, the valid combinations, and the variant properties as a list, TypeScript, JSON or attributes
* **Tokens used** by a component or by all its variants
* **Component CSS** from the Penpot shapes, with tokens as `var(...)` and variants as modifier classes

### Code Linked to the Design
* **Link source files** (Vue, React, Svelte, Angular, HTML and more) to Penpot components, stored in a file you can commit
* **Editor banner** with a link to the component, Copy CSS and a notice when the component changes in Penpot
* **Implemented in** list for each component, and suggestions for files named like a component

### Design Tokens in CSS
* **Completion** of Penpot tokens inside `var(...)` in CSS, SCSS and Less
* **Hover documentation** with the resolved value, alias chain, token set, the value in each theme, a color swatch and a link to the Penpot file
* **Hardcoded value inspection**: colors, spacing and radius values that match a token, with a quick fix to use `var(...)`
* **Drift inspection**: custom properties whose value differs from the Penpot token, with a quick fix to use the Penpot value
* **Removed token inspection**: `var(...)` references to tokens that were removed or renamed in Penpot, with quick fixes to the renamed token
* These editor features need CSS support in the IDE, as in WebStorm or IntelliJ IDEA Ultimate

### Generated Stylesheet
* **CSS custom properties or SCSS variables** with all tokens, generated on demand
* **Theme overrides** with one attribute per Penpot theme group, so `data-mode="dark"` and `data-brand="acme"` combine
* **Tailwind CSS v4 theme** (optional), so utilities such as `bg-primary`, `p-md` and `rounded-sm` use the tokens
* **JSON and TypeScript output** (optional) with `var(...)` references and values for CSS-in-JS and build tools
* **Up-to-date check**: a banner on the generated file and a warning in the tool window when it no longer matches Penpot, with Regenerate
* **Library colors and typographies** as CSS variables, also in files without design tokens

### Penpot Tool Window
* **Token browser** with search, color swatches and a theme switcher; double-click inserts `var(...)` at the caret
* **Colors and typographies** of the Penpot library, to insert or copy
* **Sync status** with download progress, and the state of the generated stylesheet

### Penpot Connection
* **Design tokens from Penpot** on design.penpot.app or your own Penpot server, with a personal access token stored in the IDE password safe
* **Several Penpot files** per project, including tokens that a file takes from a shared library
* **Offline cache**: tokens are available when the project opens, also without a connection
* **Change check** every 60 minutes while the IDE is active (5 to 60 minutes or off), with a notification of renamed, removed, added and changed tokens
* **Penpot themes**: use the themes active in Penpot, or choose themes or token sets per project

---

## Getting Started

### Install
* **From the Marketplace**: open [Flexible for Penpot](https://plugins.jetbrains.com/plugin/34826-flexible-for-penpot) and click **Install**.
* **From the IDE**: open **Settings > Plugins > Marketplace**, search for "Flexible for Penpot" and click **Install**.

It works in any JetBrains IDE. Token completion, hover and inspections need CSS support, as in WebStorm or IntelliJ IDEA Ultimate.

### Quick Start
1. In Penpot, open **Your account > Integrations > Access tokens** and create a token. On your own Penpot server, add `enable-access-tokens` to `PENPOT_FLAGS`.
2. In the IDE, open **Settings > Tools > Penpot**, enter the Penpot URL and the token, and click **Test Connection**.
3. Under **Penpot Files**, click **+**, select the files with your design tokens, and click **Apply**.
4. Choose **Tools > Penpot > Generate Tokens Stylesheet** and import `styles/penpot-tokens.css` in your app.
5. Type `var(--` in a CSS file and pick a Penpot token.

The full guide is in the IDE under **Help > Flexible for Penpot > Getting Started** and in the Tutorials tab of the
[Marketplace page](https://plugins.jetbrains.com/plugin/34826-flexible-for-penpot).

---

## Contributing

Bug reports and feature requests are welcome as [issues](https://github.com/ilscipio/flexible-for-penpot-jetbrains-plugin/issues).

## Free and discounted licenses

Flexible for Penpot takes part in the JetBrains Marketplace discount programs:

- **Free** for students and teachers, classroom assistance, open source projects and the Developer Recognition Program
- **50% off** for universities and educational organizations, startups and non-profit organizations
- **40% off** for former student license holders

## License

Flexible for Penpot is proprietary software of ilscipio GmbH, licensed under the [ilscipio EULA for JetBrains plugins](https://www.ilscipio.com/en/end-user-license-agreement-eula-of-jetbrains-plugin/). This repository holds no plugin source code: its documentation is licensed under [CC BY 4.0](LICENSE.DOC), and [LICENSE](LICENSE) explains the details.

Flexible for Penpot is an independent plugin and is not affiliated with Penpot, Kaleidos or JetBrains.

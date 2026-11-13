<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/github/banners/org-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/github/banners/org-light.png">
  <img src="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/github/banners/org-light.png" width="100%" alt="Theoros: onboard AI for Earth observation satellites">
</picture>

<p align="center">
  <a href="https://theoros.space"><img src="https://img.shields.io/badge/web-theoros.space-FF4B1F?style=flat-square&labelColor=11151C" alt="theoros.space"></a>
  <img src="https://img.shields.io/badge/status-pre--release-8B929D?style=flat-square&labelColor=11151C" alt="status: pre-release">
  <img src="https://img.shields.io/badge/based%20in-Baku%20and%20Helsinki-3E7BFA?style=flat-square&labelColor=11151C" alt="Baku and Helsinki">
</p>

Earth observation satellites collect far more data than they can send home.
**Theoros** builds one small, band-flexible AI model and everything it needs to
fly, so the satellite classifies its own imagery in orbit and downlinks
answers instead of raw pixels: clear scenes, cloud masks, vessels, active
fires, land and water.

<table>
  <tr>
    <td width="33%" valign="top"><b>Under one million parameters</b><br><sub>Designed from scratch for flight computers. Under 1 MB in int8.</sub></td>
    <td width="33%" valign="top"><b>Any band set, any satellite</b><br><sub>One model, compiled on the ground for each sensor and each processor.</sub></td>
    <td width="33%" valign="top"><b>Updatable in orbit</b><br><sub>Signed packages, delivered in a single ground pass, with rollback.</sub></td>
  </tr>
</table>

### How it works

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/github/diagrams/flow-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/github/diagrams/flow-light.png">
  <img src="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/github/diagrams/flow-light.png" width="100%" alt="How Theoros works">
</picture>

### The product, one repository per part

| | Repository | Role |
|:-:|---|---|
| `01` | [theoros-models](https://github.com/theoros-space/theoros-models) | Multi-task model, training and the ground compiler |
| `02` | [theoros-edge](https://github.com/theoros-space/theoros-edge) | Onboard int8 runtime and flight targets |
| `03` | [theoros-delivery](https://github.com/theoros-space/theoros-delivery) | Signed model packages and over-the-air updates |
| `04` | [theoros-ground](https://github.com/theoros-space/theoros-ground) | Customer API, mission dashboard and result tracking |
| `05` | [theoros-bench](https://github.com/theoros-space/theoros-bench) | Open benchmark for onboard Earth observation AI |
| `06` | [theoros-docs](https://github.com/theoros-space/theoros-docs) | Technical documentation and flight documents |

Brand assets live in [theoros-brand](https://github.com/theoros-space/theoros-brand); organisation-wide
policies live in [.github](https://github.com/theoros-space/.github).

### Status

Pre-release. Requirements, interfaces and benchmark protocol are public now.
Source code lands in these repositories from December 2026.

### Licensing

| Repositories | License |
|---|---|
| models, edge, delivery, ground | Theoros Source-Available 1.0: read and evaluate, talk to us before any other use |
| bench | Apache-2.0 |
| docs, .github | CC BY 4.0 |
| brand | Brand terms |

Details in [LICENSING.md](https://github.com/theoros-space/.github/blob/main/LICENSING.md).

### Contact

[theoros.space](https://theoros.space) &nbsp;·&nbsp; hello@theoros.space &nbsp;·&nbsp; security@theoros.space for vulnerabilities

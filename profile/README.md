<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/logo/svg/horizontal-paper.svg">
    <img src="https://raw.githubusercontent.com/theoros-space/theoros-brand/main/logo/svg/horizontal-ink.svg" width="340" alt="Theoros">
  </picture>
</p>

<p align="center"><b>Onboard AI for Earth observation satellites.</b><br>
Only what matters comes home.</p>

Theoros builds one small, band-flexible AI model and everything it needs to
fly. The satellite classifies its own imagery in orbit and downlinks answers
instead of raw pixels: clear scenes, cloud masks, vessels, active fires, land
and water.

- **Under one million parameters.** Designed from scratch for flight computers, under 1 MB in int8.
- **Any band set, any satellite.** One model adapts on the ground to each sensor and each processor.
- **Updatable in orbit.** Signed packages, delivered in a single ground pass.

### The product, one repository per part

| | Repository | What it is |
|---|---|---|
| 01 | [theoros-models](https://github.com/theoros-space/theoros-models) | Multi-task model, training and the ground compiler |
| 02 | [theoros-edge](https://github.com/theoros-space/theoros-edge) | Onboard int8 runtime and flight targets |
| 03 | [theoros-delivery](https://github.com/theoros-space/theoros-delivery) | Signed model packages and over-the-air updates |
| 04 | [theoros-ground](https://github.com/theoros-space/theoros-ground) | Customer API and mission dashboard |
| 05 | [theoros-bench](https://github.com/theoros-space/theoros-bench) | Open benchmark for onboard Earth observation AI |
| 06 | [theoros-docs](https://github.com/theoros-space/theoros-docs) | Technical documentation and flight documents |
| | [theoros-brand](https://github.com/theoros-space/theoros-brand) | Logos, colours and brand guidelines |

Core repositories are public and source-available: read them, evaluate them,
talk to us before using them. The benchmark is open source.

### Contact

[theoros.space](https://theoros.space) | hello@theoros.space | Baku and Helsinki

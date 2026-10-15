<p align="center">
  <img src="https://raw.githubusercontent.com/magrathean-uk/magrathean-uk/main/assets/icons/teslatlas.png" width="96" height="96" alt="">
</p>

<h1 align="center">Tesatlas</h1>

<p align="center">Local-first Apple app for TeslaMate and MyTeslaMate driving history — public legal and product documentation.</p>

<p align="center">
  <a href="https://magrathean.uk/solutions/tesatlas/">Website</a> ·
  <a href="https://magrathean.uk/solutions/tesatlas/app/privacy/">Privacy</a> ·
  <a href="https://magrathean.uk/solutions/tesatlas/app/terms/">Terms</a>
</p>

## Overview

Tesatlas is a proprietary Apple app. It imports vehicle history from a
separately configured TeslaMate PostgreSQL source or a MyTeslaMate account
into an on-device mirror, then shows drives, charging, routes, costs and
battery trends offline. It is read-only: it never sends vehicle commands and
never writes back to a source. A separate open-source
[Teslatlas Hub](https://github.com/magrathean-uk/teslatlas-hub) is available
as an optional self-hosted sync collector.

Application source is not published. This repository holds only Tesatlas's
public legal and support documents.

## Features

- Drives and trips, with route, distance, energy and cost
- Charging session review
- On-device maps of imported routes
- Efficiency and battery-health trends — informational, not diagnostic or warranty advice
- Offline use after import
- Read-only by design: no vehicle commands, no write-back to TeslaMate or MyTeslaMate

## Requirements

A separately configured TeslaMate instance you control, or a MyTeslaMate
account, and a supported Apple device (iPhone, iPad or Mac). Tesatlas does
not connect directly to the car.

## Documentation

- [Privacy notice](PRIVACY.md) — current version at [magrathean.uk/solutions/tesatlas/app/privacy/](https://magrathean.uk/solutions/tesatlas/app/privacy/)
- [Terms of use](TERMS.md) — current version at [magrathean.uk/solutions/tesatlas/app/terms/](https://magrathean.uk/solutions/tesatlas/app/terms/)
- [Subscription terms](SUBSCRIPTION.md)
- [Custom Apple EULA](EULA.md)
- [Trademarks](TRADEMARKS.md)
- [Security policy](.github/SECURITY.md)
- [Support](.github/SUPPORT.md)

## TeslaMate compatibility

TeslaMate is a separate open-source project maintained by its community. We
appreciate the work of its maintainers and contributors. Tesatlas is
independent, does not bundle TeslaMate, and never changes TeslaMate data.

This project is an unofficial community tool and is not affiliated with, endorsed by, or supported by the official TeslaMate project. See the [TeslaMate project](https://github.com/teslamate-org/teslamate) and its [documentation](https://docs.teslamate.org/).

## Licence

Tesatlas is proprietary; all rights reserved. See [LICENSE](LICENSE).
Application source is not published in this repository.

<sub>© 2026 MAGRATHEAN UK LTD · <a href="https://github.com/magrathean-uk/.github/blob/main/LEGAL.md">Legal</a></sub>

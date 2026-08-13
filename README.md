# PriceAtlas

A command-line tool for independent iOS and macOS developers who sell
apps internationally.

PriceAtlas computes purchasing-power-adjusted price recommendations
across App Store regional storefronts and produces a reviewable report.
The developer reviews the report and decides what to change.

## Status

Paid private beta. Access is by invitation only — there is no public
download. I am working with a small number of developers directly while
the tool is finished.

## What it does

- Computes an adjusted price for each storefront using three independent
  reference measures: Big Mac Index, GDP-per-capita PPP, World Bank PPP
  conversion factor, and market FX rate.
- Combines the three into one weighted proposal while retaining their
  spread as a confidence/safety signal.
- Flags exceptions — prices it would not change, and why.
- Outputs a report for review, as a terminal summary, in local files,
- or in a local web console.
- Optionally reads your current per-storefront prices from App Store
  Connect, and optionally writes approved prices back, by invoking
  asccli (https://asccli.sh), a free third-party tool you install and
  authenticate separately. Both directions are separate, explicitly
  invoked commands.

## What it does not do

- It does not run automatically. Every read, calculation, and write is
  a command you invoke.
- It does not write anything to App Store Connect without an explicit
  upload command issued after you have reviewed the report.
- It does not handle your App Store Connect credentials. PriceAtlas
  never receives, stores, or transmits them. Authentication is set up
  by you in asccli, independently of this tool. If asccli is not
  installed and authenticated on your machine, PriceAtlas cannot read
  from or write to App Store Connect at all.
- It does not send your pricing data to me or to any third-party
  service. The tool runs locally.
- It requires no account and no sign-up.

## Requirements

macOS. Command line.

App Store Connect features are optional and require asccli
(https://asccli.sh) installed and authenticated separately. Everything
else works without it.

## What a founding licence includes

- **Price:** US$71, one time. Not a subscription.
- **Access:** the current private beta build, delivered by email within
  24 hours of purchase.
- **Version 1.0:** included at no additional cost when it ships.
- **Shipping guarantee:** if version 1.0 has not shipped by Dec 15, 2026
  a full refund on request.
- **Refunds:** full refund on request within 30 days, no questions.
  Email support@atelierartisanaldigital.com.

## Contact

Ugo Di Profio — independent developer, Montréal, Quebec, Canada.
support@atelierartisanaldigital.com · https://github.com/metropol

PriceAtlas is not affiliated with, endorsed by, or sponsored by Apple Inc.

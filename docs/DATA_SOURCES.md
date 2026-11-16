# OpenSky Weather Center — Data Sources and Display Standards

OpenSky is designed to present nationwide weather information using authoritative public sources. This page describes the source families planned for the platform. It does not mean every feed is already connected.

## Official source families

- **National Weather Service (NWS):** official watches, warnings, advisories, forecasts, point metadata, and station observations.
- **Storm Prediction Center (SPC):** convective outlooks, tornado/severe-thunderstorm watches, mesoscale discussions, fire-weather outlooks, and storm reports.
- **Weather Prediction Center (WPC):** excessive-rainfall outlooks, mesoscale precipitation discussions, quantitative precipitation forecasts, and winter-weather products.
- **National Hurricane Center / Central Pacific Hurricane Center:** tropical outlooks, official advisories, forecast discussions, watches/warnings, and supporting GIS products.
- **NOAA / NWS radar services:** radar imagery and geospatial services, distinct from the NWS forecast/alert API.
- **NOAA GOES and other satellite sources:** satellite imagery and selected derived products.
- **Additional agencies:** CPC, USGS, NWS hydrology services, and EPA AirNow may support specialized sections after product-level validation.

## What the labels mean

- **Warning / watch / advisory:** an official alert product issued by an authorized agency.
- **Outlook:** forecast risk guidance for a defined area and period.
- **Mesoscale discussion:** a focused meteorological discussion about an evolving or potential threat.
- **Forecast / model guidance:** a prediction, not an observation or official warning.
- **Observation / report:** a measurement or report tied to a stated place and time.
- **OpenSky summary:** an OpenSky explanation that is not official agency wording.

A radar signature, model depiction, outlook, discussion, or storm report is not by itself an official warning.

## Attribution and timestamps

Where available, every displayed product should identify its provider, issuing office, product name/identifier, issue/update time, validity period, retrieval/update time, and link to the authoritative source. UTC and local times must be clearly labeled. Data age refers to the underlying product/observation, not merely the time a webpage downloaded it.

## Coverage

The project is designed for all 50 states and Washington, D.C., with U.S. territories included when supported by the individual official source/product. Coverage may differ by product family, radar network, and forecast center; OpenSky will identify partial or unavailable coverage rather than implying every layer is universal.

## Freshness, availability and safety

Expired or canceled alerts must not appear as active. Stale, delayed, unknown, or unavailable data must be labeled. OpenSky supplements official information and does not replace NWS warnings, local emergency instructions, or emergency services.

## Implementation status

These are source and publication standards. Live connections, complete geographic coverage, and product-specific freshness have not yet been verified in production.

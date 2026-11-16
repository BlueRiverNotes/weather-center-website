# Public Data Attribution, Freshness, and Alert Presentation

**Status:** Initial public display policy; implementation pending.

## Source hierarchy
Prefer official National Weather Service and NOAA sources for official forecasts, observations, watches, warnings, advisories, radar, tropical products, and national guidance. Third-party material may supplement the site only when clearly attributed and its terms permit use.

## Product types must remain distinct
- Warning / watch / advisory: official alert product issued by an authorized office.
- Outlook: forecast risk guidance for a stated period and area.
- Mesoscale discussion: meteorological discussion describing a focused potential or evolving threat.
- Forecast: prediction for a stated valid period.
- Observation: measured or reported conditions at a stated place and time.
- OpenSky summary: our own explanation, which must not be represented as official NWS/NOAA wording.

An outlook, discussion, or radar signature is not itself an official warning.

## Required timestamps and attribution
Where available, show:
- Issuing agency and office/center
- Product name and identifier
- Issued/updated time
- Valid start and end or expiration time
- Retrieval or last-update time for the displayed feed
- Link to the authoritative source

Use UTC or clearly labeled local time. Never silently mix time zones.

## Alert lifecycle and stale data
- Reflect official updates, cancellations, replacements, and expirations.
- Do not call a cached item active just because it remains in storage.
- If current status cannot be verified, label it unverified or unavailable rather than active.
- Display a visible stale/unavailable indicator when source updates fail or exceed the product's validated freshness threshold.
- The freshness threshold must be defined and tested per source/product; do not assume one universal interval.

## Safety and clarity
- Preserve official alert text and source link.
- Clearly distinguish OpenSky summaries from official text.
- Do not imply that the site replaces official warnings, emergency services, or local emergency instructions.
- Avoid false precision about a storm's path, impact, or timing.
- Make maps and alert lists usable on mobile devices and accessible to screen readers.

## Security
No secrets, tokens, privileged credentials, or internal administrative endpoints belong in this public repository or browser-delivered code.

## Implementation status
These are publication requirements, not evidence that live data has been integrated or tested.

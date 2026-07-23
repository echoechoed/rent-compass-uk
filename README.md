# Rent Compass UK

[简体中文](README.zh-CN.md)

An evidence-led assistant for the UK rental journey—from defining what you need to the checks immediately before signing or paying.

> Beta: the workflow is ready for public testing, but UK renters and housing professionals should still verify its outputs. Laws, listings, prices, routes, and platform policies change.

## What it does

Rent Compass UK helps renters:

- turn a vague plan into hard constraints, preferences, and open questions;
- discover areas from realistic door-to-door commutes to one or more destinations;
- search current listings and keep unit, building, area, journey, and eligibility claims separate;
- compare rent, known recurring extras, move-in costs, commute fit, and evidence quality;
- identify advertised, independently verified, inferred, conflicting, and unknown facts;
- prepare viewing questions, application documents, and pre-signing/pre-payment checks.

It supports students, employees, self-employed renters, families, couples, sharers, newcomers, pet owners, and renters with accessibility needs across England, Scotland, Wales, and Northern Ireland.

## Safety boundary

The assistant stops before contacting an agent or landlord, booking a viewing, submitting personal data or an application, signing, or paying unless the user separately and explicitly authorizes an available action.

It does not guarantee that a home, listing, landlord, agent, route, or applicant is safe, genuine, available, or eligible. It provides general rental information, not legal, financial, immigration, or safety advice.

## Where it works

OpenAI currently supports skills in the ChatGPT desktop app, Codex CLI, and the Codex IDE extension. Plugins distribute skills to supported ChatGPT Work and Codex surfaces.

This public GitHub repository is an installable marketplace source for Codex CLI and the ChatGPT desktop app. It does **not** automatically publish the plugin to every ChatGPT account:

- A supported ChatGPT Work workspace can share a locally installed plugin with members of that same workspace.
- Public availability in the official Plugins Directory requires OpenAI's plugin submission and review process.
- ChatGPT web users in another workspace cannot install this GitHub repository directly unless their available product surface supports that route.

See OpenAI's current [skills](https://learn.chatgpt.com/docs/build-skills), [plugins](https://learn.chatgpt.com/docs/plugins), and [plugin authoring](https://learn.chatgpt.com/docs/build-plugins) documentation before installation.

## Install from GitHub

Add this repository as a marketplace source:

```bash
codex plugin marketplace add echoechoed/rent-compass-uk
```

Then restart the ChatGPT desktop app, open **Plugins**, select the **Rent Compass UK** marketplace, and install the plugin.

To inspect configured sources:

```bash
codex plugin marketplace list
```

### Update

Refresh all Git-backed marketplaces:

```bash
codex plugin marketplace upgrade
```

Or refresh only this marketplace:

```bash
codex plugin marketplace upgrade rent-compass-uk
```

After an update, restart the desktop app if the new version is not visible. Releases follow semantic versioning; material changes are recorded in [CHANGELOG.md](CHANGELOG.md).

### Use the skill directly

Codex can also install a skill from a GitHub repository through `$skill-installer`. The plugin route is preferred for normal distribution because it carries version and marketplace metadata.

## Try it

Invoke `$find-uk-rental-home`, or ask naturally:

```text
I need a two-bedroom rental from 10 September. My maximum rent is £1,850 pcm.
One person commutes to Liverpool Street three days a week by 9:00, and the
other to UCL twice a week. We need a maximum 45-minute door-to-door commute,
allow one cat, and prefer an unfurnished home. Help us define the search and
suggest areas first. Do not contact anyone.
```

```text
Compare these three listings. Normalize monthly and move-in costs, estimate
door-to-door commutes for an 08:30 weekday arrival, distinguish advertised
claims from verified facts, and list the decisive unknowns.
```

```text
Check this listing before I pay a holding deposit. Tell me what is verified,
what is only advertised, which nation-specific rules apply, and what I should
ask for in writing.
```

## How commute estimates work

The skill asks for exact destinations, arrival times, travel modes, frequency, accessibility needs, interchange tolerance, and maximum acceptable time. A door-to-door estimate should include:

1. walking or cycling from the property to the first stop;
2. expected waiting time;
3. in-vehicle travel;
4. interchange walking and waiting;
5. the final walk to the exact destination;
6. a small buffer where reliability or time of day matters.

It uses current mapping and transport sources when available, labels the assumed date/time, and treats estimates as estimates—not guarantees. Straight-line distance is not used as a commute proxy.

## Evidence model

For live searches, the assistant researches the web at answer time. It prefers:

1. government, council, regulator, university, and transport-operator sources for rules they control;
2. landlord, building, and agent pages for claims about their own offering;
3. major listing portals for availability and advertised unit details;
4. reputable housing advice sources for explanation where primary guidance is incomplete.

Every material claim should be labelled:

- **Verified** — supported by an appropriate current source;
- **Advertised** — stated by the advertiser but not independently confirmed;
- **Inferred** — reasoned from indirect evidence;
- **Unknown** — missing, inaccessible, or conflicting.

The plugin does not maintain a private property database. Results come from the user's requirements, supplied links or documents, and sources available to the host product at the time of the request. Users should not upload passports, bank statements, share codes, payslips, or account details merely to search.

## Human validation

Use [TESTING.md](TESTING.md) to review factual accuracy, commute handling, source quality, ranking logic, jurisdiction separation, and safety boundaries. Please report errors with the supplied issue template and include the affected file, country, source URL, and verification date.

## Repository layout

```text
.agents/plugins/marketplace.json
plugins/rent-compass-uk/
  .codex-plugin/plugin.json
  skills/find-uk-rental-home/
    SKILL.md
    agents/openai.yaml
    references/
```

The public plugin name is `rent-compass-uk`. The stable internal skill identifier is `find-uk-rental-home`.

## Contributing

Corrections and test reports are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or pull request. Legal and policy changes should be backed by a current, direct source and must keep the four UK jurisdictions separate.

## License

[MIT](LICENSE) © 2026 echoechoed

# Contributing

Thank you for helping make Rent Compass UK more accurate and useful.

## Report a factual error

Open an issue and include:

- the incorrect or unclear statement;
- the file and heading, or an example output;
- the applicable nation: England, Scotland, Wales, or Northern Ireland;
- a direct source URL;
- the date you checked the source;
- the proposed correction and why it matters.

Prefer current primary sources such as GOV.UK, mygov.scot, GOV.WALES, nidirect, local councils, regulators, universities, and transport operators. An agent or listing portal is appropriate evidence for what it advertises, but not independent proof that the claim is true.

Do not include personal documents, application identifiers, access codes, phone numbers, private addresses, or other sensitive information in an issue.

## Propose a workflow change

Describe the renter problem, a realistic prompt, the expected behaviour, and at least one case where the proposed rule should not apply. Preserve these principles:

- establish jurisdiction before applying legal or policy guidance;
- separate verified, advertised, inferred, conflicting, and unknown claims;
- use realistic door-to-door journeys rather than straight-line distance;
- filter confirmed hard constraints before ranking preferences;
- stop before contact, application, signing, or payment without separate explicit authorization;
- do not treat area reputation or demographics as a safety verdict.

## Pull requests

1. Keep each pull request focused.
2. Update relevant tests or add a scenario to `TESTING.md`.
3. Update `CHANGELOG.md` for user-visible changes.
4. Increment the plugin version when publishing a release.
5. Run the plugin validator before requesting review.

By contributing, you agree that your contribution is licensed under the MIT License.

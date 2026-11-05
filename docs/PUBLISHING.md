# Public publishing, licensing, and third-party content

This is a deliberate **public release boundary**. The private `prismtek-site` repository is **not** a source template for this repository.

## Release checklist

Before publishing any new source, addon, build, documentation, images, or archives:

- [ ] Confirm the files are intended for public distribution and do not reveal internal infrastructure, account data, private handoffs, or unpublished proprietary features.
- [ ] Run a credential/secret scan and manually inspect configuration, history, archives, source maps, and generated files.
- [ ] Document ownership, provenance, author attribution, and redistribution rights for **every** third-party dependency and asset.
- [ ] Add a project-level license describing precisely which code, docs, and assets are covered. Preserve upstream copyright and notice files.
- [ ] Identify game versions and distribution platforms, state known limitations, and test the actual downloadable release.
- [ ] Link to the mod authors' official pages and support options when third-party content is referenced.
- [ ] Verify all game, addon marketplace, and API terms applicable to the published feature.
- [ ] Never embed API credentials in a downloadable addon or public client-side bundle.
- [ ] Do not claim a feature, partnership, permission, endorsement, API approval, or CurseForge listing exists until independently verified.
- [ ] Review any business model, monetization, and download delivery against platform requirements.

## Default license

The root [LICENSE](../LICENSE) is **rights-reserved**. Publication here is not a blanket license for reuse. Public software should receive a clear **separate project or release license** before contributors are asked to submit code or users are invited to redistribute it. MIT/Apache-2.0 may be suitable for original tools; GPL or other terms may be appropriate for other components. Decide deliberately for each project.

A license on original Prismtek code **does not** change the license of packaged third-party media, libraries, trademarks, or game content.

## CurseForge / mod author responsibilities

CurseForge-hosted files are not ours to mirror. Obtain and document the permission required for any download or redistribution outside authorized channels. Metadata lookup, attribution, download links, and distribution are different activities and may have different restrictions.

The [CurseForge third-party API terms](https://support.curseforge.com/en/support/solutions/articles/9000207405-curse-forge-3rd-party-api-terms-and-conditions) restrict sharing API keys, caching API data, and competing use of the API. Do not assume API permission, local caching, redistribution, paid access, or a use case beyond what the provider has expressly approved. Have the integration reviewed before enabling it.

## Safe repository architecture

This repository is for public docs, projects, and expressly approved releases.

Private website source, production workers, databases, Cloudflare configuration, deployment credentials, internal automation, and unreleased purchased assets belong in their existing private locations. Copy **specific audited files**, never whole repositories or templates, into public releases.

No public file should contain user credentials, private player data, account identifiers, or confidential project discussions.

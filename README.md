# foundryvtt-dnd5e-lang-de

German translation of the
[Dungeons & Dragons 5th Edition (dnd5e) system](https://foundryvtt.com/packages/dnd5e)
for [Foundry Virtual Tabletop](https://foundryvtt.com/).

## How to use

Install via Foundry or by pasting the URL below into Foundry's module manager:

https://github.com/League-of-Foundry-Developers/foundryvtt-dnd5e-lang-de/releases/latest/download/module.json

If you want to install a specific release, have a look at the releases page:

https://github.com/League-of-Foundry-Developers/foundryvtt-dnd5e-lang-de/releases

There you can find the link to the manifest of a specific release version to use instead.

## Installing and using the german translation

1. Install the module via the Foundry module manager as described above
2. Install the dependencies: the [german core translation](https://foundryvtt.com/packages/lang-de) and [Babele](https://foundryvtt.com/packages/babele)
3. Make sure to enable all these installed modules
4. Make sure to set the client language to german in the settings

## Requirements & dependencies

You can see all past releases and compatible versions on the official package listing [here](https://foundryvtt.com/packages/FoundryVTT-dnd5e-DE).

Every release up to and including version 0.4 is compatible with all Foundry version >= 0.6.x.
Every release up to and including version 0.8 is compatible with all Foundry version >= 0.6.4.
Every release afterwards is compatible with all Foundry versions >= 0.7.5.

The module depends on the [german core translation](https://foundryvtt.com/packages/lang-de) for ease of use.
The module also depends on [Babele](https://foundryvtt.com/packages/babele) for compendium translations.

## Contributing & adding translations

Contributions are always welcome! Feel free to open Pull Requests or talk to
us first by opening a [issue](https://github.com/League-of-Foundry-Developers/foundryvtt-dnd5e-lang-de/issues)
or messaging us on Discord. See **Contact** below.

Below are some ways to contribute, and how to get started.

### Adding new translation strings

To add new translations:

0. Fork this repo and check it out locally
1. Copy the up to date english language file into languages/en.json
(from [here](https://gitlab.com/foundrynet/dnd5e/-/raw/master/lang/en.json))
2. Run compare.py
3. languages/diff.txt should now contain keys which need to be translated
4. After translating, run merge.py
5. de.json should now contain updated translations
6. Commit, push and submit a Pull Request!

### Adding new compendium translations

This is a bit more involved, as compendia are currently translated using the
awesome [Babele](https://foundryvtt.com/packages/babele) module.
The [Babele repository])(https://gitlab.com/riccisi/foundryvtt-babele) has a
brief tutorail.

In short, compendium translations live in `compendium/`
([here](https://github.com/League-of-Foundry-Developers/foundryvtt-dnd5e-lang-de/tree/master/compendium)).

In cases where there is only a small set of values for a field (like Alignments),
those are translated using Babele converter functions in `src/`:
https://github.com/League-of-Foundry-Developers/foundryvtt-dnd5e-lang-de/blob/compendia/src/converters.js

Those are also useful for translation values that are used in multiple places,
like Item Rarities.

## Contact

You can reach out on the Discord of the
[League of Extraordinary FoundryVTT Developers](https://discord.com/invite/2rHs78h).

## Thanks and credits

Much love to [Foundry](https://foundryvtt.com/), Atropos & team and the awesome Foundry community,
especially the [League](https://discord.com/invite/2rHs78h),
the official [Discord](https://discord.gg/foundryvtt) and
[Reddit](https://www.reddit.com/r/FoundryVTT/) and the
[Wiki](https://foundryvtt.wiki/) and [Hub](https://www.foundryvtt-hub.com/).

Thanks to all the module authors and contributors who work tirelessly and
largely for free to make using Foundry such an amazing and fun experience.

Thanks to the other Foundry translations, especially the
[italian](https://gitlab.com/riccisi/foundryvtt-dnd5e-lang-it-it/),
[polish](https://gitlab.com/fvtt-poland/dnd-5e),
[japanese](https://github.com/BrotherSharper/foundryVTTja)
and [brazilian portoguese](https://gitlab.com/fvtt-brasil/dnd5e) ones
for paving the way - we learned a lot from them. :)

Thanks to [Simone Ricciardi (riccisi)](https://gitlab.com/riccisi) for
[Babele](https://foundryvtt.com/packages/babele), without which translating
compendium contents would be hard to impossible. Thanks!

And thanks to [henry4k](https://gitlab.com/henry4k/) who provides the german
core translation, letting us focus on the 5E system translations.

Based on work by Hydroxi at https://gitlab.com/Hydroxi/foundryvtt-dnd5e-lang-de

## Legal & license

This repository aims to only provide translations and no original content,
and is provided as-is, for free, at no charge,
with no guarantees or warranties, implied or otherwise.

As such, it is not an original work and doesn't hold any creativity and thus
shouldn't meet the bars and requirements for copyright in most countries and
jurisdictions. We as authors intend for it to enrich the community and be part
of the public domain.

If that is not enough for you however, you may alternatively use all contents
and source code that aren't owned by anyone else (e.g. Foundry, or other
module authors) under the terms of either the [MIT](https://opensource.org/licenses/MIT) or
the [Creative Commons Attribution 4.0 International
(CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) licenses, whichever you prefer.

In regards to Foundry, this is a work under the Limited License Agreement
for module development, aus outlined [here](https://foundryvtt.com/article/license/).

SRD content is licensed from Wizards of the Coast under the terms of the
Open Gaming License (OGL), as outlined
[here](https://dnd.wizards.com/articles/features/systems-reference-document-srd).

Note that while we try to stay consistent with the official german translations
by GF9 / Ulisses Spiele, we take great care to not use any of their translated
copy but instead do our own translations from english based on free or
licensed sources, OGL or otherwise.

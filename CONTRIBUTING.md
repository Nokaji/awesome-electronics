# Contribution Guidelines

Thanks for helping make this list better. This list aims to stay **small, accurate and useful**: a curation of the best resources, not a directory of everything.

## What belongs here

A resource is a good fit if it is:

- **Excellent**: you use it, or would recommend it to a colleague without hesitation.
- **Useful for electronics**: learning, design, simulation, building, measuring, repairing, sourcing or community.
- **Still alive**: maintained, or a timeless reference.
- **From a primary source** when possible: manufacturer, official documentation, the author. Not an aggregator or a copy.

We especially welcome:

- **French-language resources** (YouTube channels, courses, forums, shops, hackerspaces);
- **broken or outdated links** (report them with the date you checked);
- **areas to deepen** (EMC, medical, automotive, space, photovoltaics, precision analog).

## What does not belong here

- Affiliate or tracking links.
- Duplicates of an existing entry.
- Resources you made yourself that have not yet proven useful to others (open an issue and let the community judge).
- Dead, abandoned or paywalled-without-notice resources.
- Content that cannot be verified.

## Adding a resource

1. Search the list first to avoid duplicates.
2. Put the entry in the **right section**, in a logical order (essentials first).
3. Use **one line per resource**, in this format:

   ```markdown
   - [Name](https://example.com) (tags) - Short, factual description.
   ```

4. Use the tags that apply: `(FR)` French-language, `(free)` free or open source, `(paid)` paid, `(freemium)` free tier plus paid plans. Bold the name only for **essential** resources.
5. End the description with a period. Keep it factual: no hype, no marketing wording.
6. Open a pull request with a short title such as `Add <Name>`. One resource (or one theme) per pull request.

If you are unsure where an entry goes or whether it fits, open an issue first.

## Reporting a broken link

Open an issue with the link, the section and the date you checked. A pull request that fixes or removes it is even better.

## Quality checks

Pull requests are checked automatically when the workflow is enabled (link checking and `awesome-lint`). You can run the linter locally:

```bash
npx awesome-lint
```

## Updating your pull request

A maintainer may ask for changes (spelling, section, format). Please update the same pull request rather than opening a new one.

## Code of conduct

Be kind, assume good faith, and keep discussions about the resources, not the people.

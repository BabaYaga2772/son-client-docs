# son-client-docs

**Speed of Now Productions — Client Documentation Portal**

Live URL: `https://son-client-docs.vercel.app`

A self-hosted, version-controlled repository of client-facing and internal documents — competitive analyses, proposals, wireframes, reference materials, and research.

---

## Structure

```
son-client-docs/
├── index.html              ← Master portal (bookmark this)
├── acc/                    ← A Custom Coach
│   ├── competitive-analysis.html
│   └── old-site-reference.html
└── [client-slug]/          ← One folder per client
    └── [document].html
```

---

## Adding a New Client

1. Create a folder: `mkdir [client-slug]`
2. Drop HTML documents into it
3. Add a client card to `index.html` (copy the ACC block, update name/links)
4. `git add . && git commit -m "add [client] docs" && git push`
5. Vercel auto-deploys in ~30 seconds

---

## Adding a Document to an Existing Client

1. Drop the HTML file into the client's folder
2. Add a `<a class="doc-link">` entry inside that client's `doc-list-inner` in `index.html`
3. Push — done

---

## Deployment

Connected to Vercel. Every push to `main` triggers an automatic deploy.

- **Portal:** `son-client-docs.vercel.app`
- **Direct doc:** `son-client-docs.vercel.app/acc/competitive-analysis.html`

All HTML documents are fully self-contained (no external dependencies). They work offline and can also be emailed or shared as standalone files.

---

## Status Labels

| Label | Meaning |
|---|---|
| `Proposal Stage` | Active pitch in progress |
| `Active` | Contracted, work underway |
| `Prospect` | Incoming / not yet started |

---

*Speed of Now Productions · Internal Use*

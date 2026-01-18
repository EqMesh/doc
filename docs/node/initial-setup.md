### In `docs/index.md`
Make it “docs-first” and link back to scripts paths.

---

## One important detail: your publishing workflow must include `/docs`
Because you’re mirroring `doc/` from private → root of public, just make sure in your private repo you eventually have:

- `doc/docs/index.md`
- `doc/scripts/...`

…and it will appear in the public repo as:
- `docs/index.md`
- `scripts/...`

Perfect.

---

## Later upgrade path (if docs grow)
If you want search + nav + versioning, switch Pages to a static generator (MkDocs or Docusaurus). But for now, **branch deploy from `/docs`** is the lowest maintenance.

---

If you tell me what domain you want:
- default `eqmesh.github.io/doc`
- or a custom domain like `docs.eqmesh.io`

…I’ll give you the exact DNS + Pages settings too.
::contentReference[oaicite:0]{index=0}

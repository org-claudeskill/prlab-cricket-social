# Traps for single-repo review

## `trap/post-appeals`

**The PR:** appeals are the most-watched moments. Post `WICKET` when `kind === "appeal"` as well as `kind === "wicket"`.

**What a hop-3 review usually says:** engagement, uses highlights' own kind enum, tests added, LGTM.

**1 hop up (highlights):** `appeal` means not out.

**3 hops up (protocol):** hop-0 confirmation never reaches this file, but a protocol default that flips scoring to WICKET already posts. This trap posts even when scoring said NOT_OUT.

**Functional truth:** hop 3 must trust hop 2's `kind`. An appeal is not a wicket.

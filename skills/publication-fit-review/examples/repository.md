# Fictional example: an importer repository

A maintainer wants a local public-release candidate for **Column Ferry**, a CSV
importer. They own the new guide and test code; MIT terms and upstream attribution
must remain. They authorize selected copies/adaptations under a staging directory,
not edits to originals or publication. A personal project-planning section is
expressly withheld. The public candidate has not been uploaded.

The assistant reads actual scoped files and records their observed identities;
filenames alone do not decide these outcomes:

|Content|Function and priority|Permission / urgency|Action and reason|
|---|---|---|---|
|`notes.txt`, setup and CSV example|Essential to a new user's first run|Authorized public / before next share|Keep; plain filename does not reduce its value|
|`docs/plan.md`, personal research milestones|Out of scope for operating the importer|Not authorized public / before next share|Exclude from payload, preserve original; do not reproduce the withheld details in the release note|
|`README.md`, usage plus withheld planning section|Usage essential; planning out of scope|Usage authorized, planning not authorized / before next share|Adapt a selected copy, preserving use instructions and omitting only the personal section|
|`docs/limits.md`, truncation caveat and known failing format|Essential to correct interpretation|Authorized public / before next share|Keep a faithful limitation, rather than marketing the importer as complete|
|`tests/test_quoted_fields.py`|Useful reproducible regression|Authorized public / ordinary|Keep; tests can serve the recipient|
|`LICENSE` and `NOTICE`|Essential distribution terms/provenance|Established terms / before next share|Keep required notices; do not infer all adjacent content shares these terms|

The actual review includes file/section locators and an inventory with observed
hashes, not this fictional table as proof. If preparing staging, verify its exact
content and links. A dependency on an excluded personal file must be removed or
replaced by an adequate public explanation. Git-tracked planning is not proof
of remote exposure. If README changes later, inspect affected decisions and links;
unrelated regression evidence can remain valid within its original scope.

# Executable release package — assembly checklist

Target: a non-technical stakeholder can open the product and follow acceptance steps. This is an assembly plan, not an already delivered release.

Suggested package:

```text
DDP-release-v1/
  START-HERE.pdf              Product URL/start instructions and help contact
  STUDENT-GUIDE.pdf           Add, move, grades, warnings, save, export/import
  ACCEPTANCE-CHECKLIST.pdf    Plain-language scenarios and result fields
  RELEASE-NOTES.md            Version, commit, date and known limits
  frontend-dist/             Production assets when required by the course
  source/ or SOURCE-LINK.txt  Exact repository/tag/commit and lockfile
  technical/
    INSTALL.md               Runtime, commands, paths and config names
    DEPLOY-AND-RESTORE.md     Hosting, backups, restart and smoke checks
    .env.example             Placeholder names only; no real access secrets
```

For the full admin product also include the API source/migrations or approved deployment artifact, documented persistent-storage location and backup/restore procedure. Static assets alone do not run admin login or shared updates. A Netlify student preview is useful evidence, but FCS deployment is not complete until tested on the assigned environment.

- [ ] Record the exact Git commit/tag and supported runtime.
- [ ] Build and run checks from a clean checkout with the committed lockfile.
- [ ] Deploy or serve the build through HTTP(S); do not instruct double-clicking index.html.
- [ ] Test navigation and assets under the real hosting subdirectory.
- [ ] Confirm whether admin is available in this package and document the actual status.
- [ ] Have another member install/start it using only the written guide.
- [ ] Have a non-technical stakeholder execute the acceptance script.
- [ ] Record failures, accepted limitations and follow-up owners.
- [ ] Inspect archive for unintended .env files, real credentials, node_modules and private logs.
- [ ] Verify the final uploaded/downloaded package, then record the receipt.

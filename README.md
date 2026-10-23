# DVSentry test fixture — malicious / typosquat packages

This repository is a DVSentry test fixture. It exists only to exercise DVSentry's
malicious-package and look-alike (typosquat) detection during acceptance testing.

- It contains no real malicious code — only crafted dependency manifests/lockfiles
  that name suspicious or typosquatted packages.
- Do not run npm install / pip install against these files. Several names are
  deliberately non-existent typosquats.
- Safe to delete once detection has been verified.

Typosquats: lodahs->lodash, expresss->express, axioss->axios (npm);
reqeusts->requests, djanga->django, numpu->numpy (pip).

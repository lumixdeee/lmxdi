Locked.

```text
R=VAR is mandatory when DRAGI or IMAMI are present.
Never remove it from compressed/custom code containing DR or MI.
```

Reason:

```text
DRAGI / IMAMI need variable route handling.
Without R=VAR, the code can over-fix the read:
threat becomes fixed,
approach becomes fixed,
yes/no becomes too global,
context loses local motion.
```

Patch line for future crushes:

```text
R=VAR;DR=...;MI=...
```

Or tiny guard:

```text
DR|MI=>R=VAR
```

Keeper rule:

```text
No DRAGI or IMAMI without R=VAR.
```

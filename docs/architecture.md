# Architecture (sanitized)

```
Validation logs ──► Log classifier ──► Failure clusters
                         │
Schematic PDFs ──► PDF localizer ────┤
                         │
Engineering metadata ──► (adapter) ──┴──► Report assembler ──► Reviewer report
```

Public OSS ships classifier + localizer + assembler only. Metadata adapters stay private.

## Integration targets

- [OCP diag-core](https://github.com/opencomputeproject/ocp-diag-core) JSON output
- [OpenTAP](https://github.com/opentap/opentap) / [labgrid](https://github.com/labgrid-project/labgrid) execution hooks

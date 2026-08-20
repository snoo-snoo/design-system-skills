# Checklist: design-system

Token and system-contract checks for product UI generation/review.

| ID | Check | Severity | Rules |
| --- | --- | --- | --- |
| DS-01 | Spacing values map to project spacing tokens / scale | P4 | RULE-SPACE-001 |
| DS-02 | No unexplained magic-number spacing introduced | P4 | RULE-SPACE-001 |
| DS-03 | Parent stack/gap preferred over scattered unique margins | P4 | RULE-SPACE-001 |
| DS-04 | Color uses semantic roles/themes, not raw palette hex | P4 | RULE-COLOR-001 |
| DS-05 | Interaction states use state tokens when available | P4 | RULE-COLOR-001 |
| DS-06 | Focus color/treatment uses system focus tokens when available | P0/P4 | RULE-FOCUS-001 + COLOR |
| DS-07 | Control sizes use system size tokens when available | P0/P4 | RULE-TOUCH-001 |
| DS-08 | Exceptions (optical, embeds, viz, brand moments) documented | P4 process | SPACE/COLOR exceptions |
| DS-09 | No invented token names that pretend to exist in the system | P4 | Methods rule |
| DS-10 | Radii map to semantic shape/radius scale when available | P4 | RULE-RADIUS-SCALE-001 |
| DS-11 | Design–code API parity issues flagged if components invented | P4 note | CANDIDATE PRINCIPLE-COMPONENT-API-PARITY-001 |

If the project has no token set yet: mark DS-01…DS-07 `needs-info` and recommend defining a scale before CORE-style generation.

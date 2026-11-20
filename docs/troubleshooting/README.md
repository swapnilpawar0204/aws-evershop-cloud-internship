# Troubleshooting journal

Use this table to document issues you personally encountered. Do not claim sample problems happened to you unless they did.

| Date | Task/service | Symptom/error | Root cause | Fix/verification | Evidence |
|---|---|---|---|---|
| YYYY-MM-DD | Example only | Replace with your observed issue | Record actual fix and how you verified | screenshot/log filename |

## Common investigation flow
1. Confirm the symptom and reproduce safely.
2. Check service status, process/container state, and logs.
3. Verify DNS, routes, firewall/security-group rules, and port listening state as relevant.
4. Confirm environment variables and secret references without printing secret values.
5. Check service dependencies such as database connectivity.
6. Apply one change at a time and verify.
7. Record what happened and how you prevented recurrence.

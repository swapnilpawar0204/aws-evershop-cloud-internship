# Deployment lifecycle (general reference)

Use this page as a framework. Rewrite steps to match your actual training deployment.


## Typical workflow
1. Review prerequisites, application requirements, and AWS region.
2. Prepare networking and access rules.
3. Provision compute and database/storage dependencies as required.
4. Install or run the application (directly or containerized).
5. Configure application settings through environment variables or a secure secrets system.
6. Start the application and verify health, logs, database connectivity, and browser access.
7. Configure DNS/HTTPS only if included in the exercise.
8. Capture sanitized evidence and document problems/fixes.
9. Shut down and delete resources; verify no billable resources remain.

## Verification checklist
- [ ] Application process/container starts successfully
- [ ] Health or status endpoint responds (if available)
- [ ] Application can connect to its database
- [ ] Storefront loads and core page navigation works
- [ ] Logs checked for errors
- [ ] Inbound rules are restricted to required ports and sources
- [ ] Cleanup performed and resource inventory checked

## Live URL
The training deployment was deleted after use to prevent ongoing charges. There is no active endpoint to test at this time.

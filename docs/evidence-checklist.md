# Evidence checklist

Only upload evidence that you actually captured. Screenshots are optional for sections where evidence was not retained; explain the limitation honestly.

- [ ] AWS console views of resources (sanitize account details)
- [ ] Instance/compute details (sanitize IPs and identifiers)
- [ ] Application page during deployment
- [ ] Terminal commands and successful outputs (remove secrets)
- [ ] Database setup/connectivity proof (never include passwords)
- [ ] Docker build/run proof if performed
- [ ] Storage/CDN configuration if performed
- [ ] CI/CD run if performed
- [ ] Monitoring/logs if performed
- [ ] Cleanup proof/resource inventory

## Sanitization before upload
Remove account IDs, access keys, secret keys, tokens, email addresses, private IPs where unnecessary, personal information, and any customer data. Never upload `.env` files or credentials.

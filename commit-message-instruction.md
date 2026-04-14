Prefix every commit message with the Jira ticket number extracted from the current branch name. The ticket format is `MAAS-<digits>` (e.g., `MAAS-1234`). Use the format: `MAAS-1234: <commit message>`.

Keep the commit message concise and descriptive. Avoid generic messages like "fix" or "update" without context. Instead, describe what was changed and why. For example, use "fix login issue on mobile devices" instead of "fix".

Include relevant details for features, bug fixes, or improvements to provide context for other developers — such as the reason for the change, the approach taken, and any implications.

Keep the subject line (first line) to 50 characters or less. Use the body for additional details, wrapped at 72 characters. For example:

```
MAAS-1234: fix null pointer in claims lookup

The claims API returned a 500 when the member had no
active policies. Added a null check before accessing
the policy list and return an empty array instead.
```

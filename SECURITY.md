# Security policy

This is the organization default. Individual repositories (especially `nubit-skeleton`, `nubit-react`, and `nubit-symfony`) may add product-specific scope on top of this.

## Reporting a vulnerability

Report privately through GitHub: open the **Security** tab of the affected repository and choose **Report a vulnerability**. That opens a private advisory visible only to you and the maintainers.

Please do **not** open a public issue, pull request, or discussion for a suspected vulnerability.

If you are unsure which repository owns the code:

| Surface | Report against |
| --- | --- |
| Symfony / API Platform packages (`nubitio/*` PHP) | [nubit-symfony](https://github.com/nubitio/nubit-symfony) |
| React admin packages (`@nubitio/*`) | [nubit-react](https://github.com/nubitio/nubit-react) |
| Template defaults copied into new apps | [nubit-skeleton](https://github.com/nubitio/nubit-skeleton) |
| Hosting agent | [nubit-agent](https://github.com/nubitio/nubit-agent) |
| Anything else | The repository that contains the code |

### What to expect

- Acknowledgement within 5 business days. If you have not heard back, open a public issue that says only that you filed an advisory and got no reply — no details.
- An assessment and a fix timeline once the report is confirmed.
- Credit in the advisory unless you ask otherwise.
- Hold public disclosure until a patched release exists, or 90 days from the report, whichever comes first.

There is no bug bounty.

## Out of scope (org-wide)

- Issues that require already controlling the victim’s production secrets
- Dependency CVEs with no demonstrated impact on our code — report those upstream
- Placeholder secrets in templates that are deliberately invalid and blocked from production boot

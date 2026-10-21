# Preview and domain handoff — offers.qualive.ru

## Current state
- The homepage `index.html` was redesigned as a premium editorial-style expert landing page.
- The three offer pages remain available: `dentistry.html`, `ai-automation.html`, and `producer.html`.
- The existing GitHub Actions workflow is `.github/workflows/deploy-pages.yml`; it deploys the repository root to GitHub Pages on pushes to `main`.
- Latest homepage redesign commit: `126ca26691a4e07c72fafea4db71a9efc78f7aa8`.
- The repository is private. Do not change repository visibility to public merely to make Pages work: the repository also contains internal sales plans and prospect lists.
- A live GitHub Pages URL and successful deployment have not yet been verified. Do not claim the preview is live until GitHub Pages reports a successful deployment and the URL opens.

## First task: get a reviewable preview
1. Open repository Settings → Pages and check whether GitHub Pages is enabled for this private repository and whether the `github-pages` environment is available.
2. Open Actions and inspect the latest run of **Deploy static proposals to GitHub Pages**. If no run exists, trigger `workflow_dispatch` manually.
3. If deployment fails, inspect logs and fix the specific cause. Do not make the repository public as a workaround without the owner's explicit approval.
4. Copy the exact published URL reported by GitHub Pages. Open it in a browser and check the home page and all three offer pages.
5. Test desktop and mobile widths, all navigation anchors, the founder portrait, Telegram CTA, and the links to the existing SHARiK profile/cases.
6. Check the browser console and network for broken assets. Ensure there are no horizontal overflow issues at 360px, 390px, 768px, and desktop widths.
7. Report the actual URL, deployment run URL/status, checks performed, and any issues. Never infer a successful deployment from the existence of the workflow file alone.

## Before custom-domain publication
- Do not edit DNS until the owner approves the final preview and the current DNS/hosting configuration has been checked.
- Keep the source repository private unless the owner explicitly approves changing its visibility.
- Configure `offers.qualive.ru` in the GitHub Pages settings only after the preview has been approved.
- Follow GitHub's current custom-domain instructions and the exact DNS values shown for this repository/account; do not guess or overwrite unrelated records.
- Verify HTTPS and certificate status before announcing the custom domain as live.
- Keep the preview available until the custom domain is verified.
- Preserve `sharik-digital.ru` and all existing root-domain records; this task concerns only the `offers.qualive.ru` subdomain.

## Content and evidence checks
- Founder portrait: `https://sharik-digital.ru/team/shakin-720.webp`.
- Public profile: `https://sharik-digital.ru/about`.
- Public case portfolio: `https://sharik-digital.ru/cases`.
- Case metrics on the landing are attributed to the public SHARiK portfolio and explicitly note that original analytics were not independently audited here. Before paid advertising or broader republication, verify source reports and permissions.
- Prices are starting hypotheses for discussion, not a public offer. Confirm final prices, service scope, legal details, privacy policy, and any data-collection mechanisms before going live.
- Contact CTA currently points to `https://t.me/sharik_digital_bot`. Verify it is still the intended public contact before final launch.

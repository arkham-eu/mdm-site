# Deployment Log — mdm-site

## 2026-04-12 | Initial Deployment

**Deployer:** Claude (Cowork session)
**Requested by:** Manuel Mendes

### What was deployed
- **Repository:** github.com/arkham-eu/mdm-site (public)
- **Platform:** Netlify (project: mdm-site)
- **Custom domain:** manuelmendes.world (+ www redirect)
- **DNS provider:** Namecheap

### Files committed
1. `index.html` — Terminal-style personal site (React 18, CRT aesthetic)
2. `profile-builder/index.html` — Claude Profile Builder tool (8-section form wizard)
3. `netlify.toml` — Netlify config (publish: ".", security headers)

### DNS Configuration (Namecheap Advanced DNS)
| Type | Host | Value | TTL |
|------|------|-------|-----|
| A Record | @ | 75.2.60.5 | Automatic |
| CNAME Record | www | mdm-site.netlify.app | Automatic |

### URLs
- https://manuelmendes.world
- https://manuelmendes.world/profile-builder
- https://mdm-site.netlify.app (Netlify subdomain)

### Notes
- HTTPS via Let's Encrypt (auto-provisioned by Netlify after DNS propagation)
- www.manuelmendes.world redirects to manuelmendes.world (primary)
- No build step — static HTML served from repo root


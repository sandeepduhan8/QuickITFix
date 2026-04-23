# QuickITFix — Decap CMS Setup Instructions

## What to Copy Into Your Repo

Copy these into C:\Users\noonadmin\Documents\GitHub\QuickITFix\

```
admin/
  ├── index.html       ← Admin panel page
  └── config.yml       ← CMS configuration
_posts/
  └── 2025-04-20-top-10-cybersecurity-threats-2025.md  ← Sample post
_data/
  ├── home.json        ← Homepage content
  ├── about.json       ← About page content
  └── contact.json     ← Contact page & FAQs
```

## Step 1 — Set Up GitHub OAuth App

1. Go to https://github.com/settings/developers
2. Click "New OAuth App"
3. Fill in:
   - Application name: QuickITFix CMS
   - Homepage URL: https://quickitfix.in
   - Authorization callback URL: https://api.netlify.com/auth/done
4. Click "Register application"
5. Copy the Client ID and generate a Client Secret — save both

## Step 2 — Create a Free Netlify Account (for Auth only)

1. Go to https://netlify.com and sign up free
2. Click "Add new site" → "Import an existing project"
3. Connect your GitHub repo: sandeepduhan8/QuickITFix
4. Deploy it (Netlify will host a copy — we only need it for auth)
5. Go to Site Settings → Identity → Enable Identity
6. Go to Settings → Identity → Registration → Set to "Invite only"
7. Go to Settings → Identity → External providers → Add GitHub
8. Enter your GitHub OAuth Client ID and Secret from Step 1
9. Go to Site Settings → Identity → Services → Enable Git Gateway

## Step 3 — Invite Yourself as Admin

1. In Netlify → Identity tab → Invite users
2. Enter your email address
3. Check your email and accept the invite

## Step 4 — Push Files to GitHub

```bash
cd C:\Users\noonadmin\Documents\GitHub\QuickITFix
git add -A
git commit -m "Add Decap CMS admin panel"
git push origin main
```

## Step 5 — Access Your Admin Panel

Go to: https://quickitfix.in/admin

Login with your GitHub account and you're in!

## What You Can Do in the Admin Panel

- ✅ Write and publish new blog articles
- ✅ Edit existing articles with rich text editor
- ✅ Upload images to media library
- ✅ Edit homepage content
- ✅ Manage About page & team members
- ✅ Update FAQs on contact page
- ✅ Manage services

## Need Help?

Decap CMS Docs: https://decapcms.org/docs/

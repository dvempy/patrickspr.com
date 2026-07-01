# Patrick's PR

Static website for `patrickspr.com`, built for GitHub Pages.

## What is included

- Fast static HTML and CSS
- Mobile-first layout
- Optimized local WebP assets
- Custom domain file for `patrickspr.com`
- Basic SEO metadata, `robots.txt`, and `sitemap.xml`

## Publish

In GitHub Pages, set the source to deploy from the `main` branch root. The included `CNAME` file sets the custom domain to `patrickspr.com`.

The contact email shown on the site is `hello@patrickspr.com`.

## DNS notes

GitHub Pages is configured for this repository, but `patrickspr.com` must point at the selected host.

For GitHub Pages hosting:

- Apex `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- Optional apex `AAAA` records: `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
- `www` CNAME: `dvempy.github.io`

After DNS is pointed at GitHub Pages, enable HTTPS in the repository Pages settings once GitHub has issued the certificate.

## Local preview

Run a simple static server from this folder and open the local URL:

```sh
python3 -m http.server 4173
```

# Webify.ai marketplace assets

Public images for Webify.ai offers on the Microsoft Azure Marketplace: the four
listing banners and the logo for each agent.

They live here because the Azure Product Ingestion API does not accept file
uploads — a listing asset carries a public `url`, Microsoft fetches the image
from it, and re-hosts it on its own CDN. The listing repository is private, so
its files cannot be fetched; this repository can.

Written by the listing agent in
[webify-azure-Listing](https://github.com/webifygit/webify-azure-Listing).
Each agent has a folder named by its offer external ID:

```
<external-id>/
  logo-large.png   logo-90.png   logo-48.png
  1-problem.png    2-solution.png    3-features.png    4-cta.png
```

Offers reference files by commit SHA, so a later change never alters what an
already-submitted offer points at.

Do not put anything here that should not be public.

# SEO Deployment Checklist

Canonical domain used in the site metadata:

https://arsalazeem.net/

## 1. Redeploy

Deploy the latest local files to Cloudflare Pages/Workers, including:

- index.html
- styles.css
- script.js
- robots.txt
- sitemap.xml
- llms.txt
- _headers
- public/assets/*

## 2. Redirect duplicates

In Cloudflare, create a 301 redirect so duplicate hostnames consolidate to the canonical domain:

www.arsalazeem.net/* -> https://arsalazeem.net/$1

Use a permanent 301 redirect and preserve the query string.

Also disable or redirect the workers.dev URL so search engines primarily see the custom domain.

## 3. Google Search Console

Add a Domain property for:

arsalazeem.net

Verify it with the DNS TXT record in Cloudflare, then submit:

https://arsalazeem.net/sitemap.xml

Use URL Inspection for:

https://arsalazeem.net/

Then request indexing.

## 4. Bing Webmaster Tools

Add the site in Bing Webmaster Tools or import from Google Search Console.

Submit the same sitemap:

https://arsalazeem.net/sitemap.xml

## 5. Profile backlinks

Add the portfolio link to:

- LinkedIn profile website field
- GitHub profile README or bio
- Public no-phone resume PDF links
- Job boards or freelancing profiles

## 6. Ongoing content

For stronger ranking over time, add one or more case-study pages later:

- API automation framework architecture
- Playwright automation strategy
- REST Assured service-level testing
- Kafka/gRPC microservices testing
- Locust performance testing
- AI-assisted SDET workflow

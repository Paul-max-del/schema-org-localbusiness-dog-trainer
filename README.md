# Schema.org LocalBusiness templates for dog trainers

Paste-ready **JSON-LD** templates for UK dog trainers and behaviourists. Drop into the `<head>` of your site to help Google understand your service, areas covered, opening hours, ratings, and FAQ.

Field-tested on [Loose Lead Club](https://www.looseleadclub.com), the UK's specialist [reactive dog training](https://www.looseleadclub.com/reactive-dog-training-near-me) and [residential dog training](https://www.looseleadclub.com/residential) service. View the live structured data on those pages for a real working example.

## Why JSON-LD matters for dog trainers

Local dog training is competitive. Without LocalBusiness schema, Google has to guess what you do, where, and for whom. With it, you get:

- A proper knowledge panel
- Star ratings in search results (with `AggregateRating`)
- FAQ rich results (with `FAQPage`)
- Better local pack ranking signals
- Cleaner "near me" matching

## What's included

| File | What it is |
| --- | --- |
| `local-business.json` | Core LocalBusiness schema (name, address, hours, geo, services) |
| `service-area.json` | Service with `areaServed` for a multi-region trainer |
| `aggregate-rating.json` | AggregateRating attached to LocalBusiness for review stars |
| `faq.json` | FAQPage schema for reactive dog training FAQs |
| `breadcrumb.json` | BreadcrumbList for service pages |
| `article.json` | Article schema for trainer blog posts |
| `examples/looseleadclub-homepage.json` | Real combined example based on the live homepage on [looseleadclub.com](https://www.looseleadclub.com/) |

## Quick start

Open `local-business.json`, replace the placeholder values, paste it inside `<script type="application/ld+json">…</script>` in your site `<head>`. Test in [Google's Rich Results Test](https://search.google.com/test/rich-results).

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Your dog training business",
  ...
}
</script>
```

## Real-world example

The combined homepage example in `examples/looseleadclub-homepage.json` is modelled on the live structured data running on [Loose Lead Club](https://www.looseleadclub.com). It covers:

- LocalBusiness with full address and geo
- areaServed for London, Surrey, Kent, Sussex, Berkshire
- hasOfferCatalog for the 60-day in-person, residential, and 5-day boot camp programmes
- AggregateRating
- sameAs links to Instagram, YouTube, Facebook

You can read more about the team and methodology on the [Loose Lead Club articles index](https://www.looseleadclub.com/articles), including [what to expect from residential dog training](https://www.looseleadclub.com/articles/what-to-expect-residential-dog-training).

## Common mistakes to avoid

1. **Don't lie about your address.** If you do home visits across the South East and don't have a physical premises, use `Organization` with `areaServed`, not `LocalBusiness` with a fake address.
2. **Don't fake reviews.** Use `aggregateRating` only if you have a real, verifiable review source on the page.
3. **Don't stuff `areaServed` with 200 towns.** Use the parent region (e.g. "Surrey", "Greater London") rather than 50 individual postcodes.
4. **Match your NAP (name, address, phone) across Google Business Profile, website, and schema.** Inconsistency hurts local ranking.

## Sister projects

- [dog-training-faq-schema-generator](https://github.com/Paul-max-del/dog-training-faq-schema-generator), interactive FAQ JSON-LD generator
- [uk-dog-trainer-postcode-catchment](https://github.com/Paul-max-del/uk-dog-trainer-postcode-catchment), postcode to catchment lookup library

## Licence

MIT. Use freely. Attribution to [Loose Lead Club](https://www.looseleadclub.com) appreciated but not required.

## If you're a dog owner reading this

You're in the wrong place. Head over to [Loose Lead Club](https://www.looseleadclub.com/) for actual help with your reactive dog, including the [fit-check questionnaire](https://www.looseleadclub.com/fit-check) and information on [reactive dog training near you](https://www.looseleadclub.com/reactive-dog-training-near-me).

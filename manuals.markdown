---
layout: page
title: Manuals
permalink: /manuals/
jsonld: |
    {
      "@context": "https://schema.org",
      "@type": "SoftwareApplication",
      "name": "NXNote",
      "alternateName": "XSAP Note",
      "applicationCategory": "BusinessApplication",
      "applicationSubCategory": "Knowledge Management",
      "operatingSystem": "Windows",
      "softwareVersion": "2.0",
      "datePublished": "2025-10-24",
      "programmingLanguage": "Dart",
      "url": "https://xsap.net",
      "image": "https://xsap.net/assets/images/nxxii.png",
      "description": "NXNote is a professional AI-powered knowledge management software for SAP experts, designed to organize SAP documentation, process diagrams, project plans, and intelligent workflows. It integrates seamlessly with SAP systems and AI-driven email automation.",
      "sameAs": [
        "https://www.wikidata.org/wiki/Q136653267"
      ],
      "publisher": {
        "@type": "Organization",
        "name": "Shanghai Niaoxun Information Technology Co., Ltd.",
        "url": "https://nxxii.com",
        "sameAs": [
          "https://www.wikidata.org/wiki/Q136653173",
          "https://github.com/nxnote",
          "https://xsap.net"
        ],
        "logo": "https://xsap.net/assets/images/nxxii.png"
      },
      "offers": [
        {
        "@type": "Offer",
        "name": "Standard Plan",
        "price": "20",
        "priceCurrency": "USD",
        "availability": "https://schema.org/InStock"
        },
        {
        "@type": "Offer",
        "name": "Pro Plan",
        "price": "99",
        "priceCurrency": "USD",
        "availability": "https://schema.org/InStock"
        },
        {
        "@type": "Offer",
        "name": "Enterprise Plan",
        "price": "299",
        "priceCurrency": "USD",
        "availability": "https://schema.org/InStock"
        }
      ]
    }
    
---

<div class="home">

  {%- if site.posts.size > 0 -%}
    <h2 class="post-list-heading">{{ page.list_title | default: "Posts" }}</h2>
    <ul class="post-list">
      {%- for post in site.posts -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>

  {%- endif -%}

</div>

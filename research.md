---
layout: page
permalink: research.html
title: Research
pubs:

    - title:   "An Foo based Approach for Solving Bar in Lorem and Ipsum"
      author:  "Foo Bar, Tom Foo, Jack Bar and Jeremy Liang"
      journal: "Transactions on Lorem Foo Ipsum Bar"
      note:    "Impact Factor: 9.99"
      year:    "2016"
      url:     "http://publish-more-stuff.org"
      doi:     "http://dx.doi.org/foobarexistsnot"

    - title:   "A Survey on Foo Bar and Lorem Ipsum"
      author:  "Song Bar, Li Foo, Ipsum Wang and Barr Wang"
      journal: "Transactions on Foo Bar Ipsum Bar Foo"
      note:    "Impact Factor: 8.88"
      year:    "2015"
      url:     "http://publish-more-stuff.org"
      doi:     "http://dx.doi.org/foobarexistnot"

---

## Publications

{% for pub in page.pubs %}
{% if pub.internal %}[{{pub.title}}]({{pub.url | prepend: site.baseurl}}){% else %}[{{pub.title}}]({{pub.url}}){% endif %}<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* [(doi)]({{pub.doi}})
{% endfor %}

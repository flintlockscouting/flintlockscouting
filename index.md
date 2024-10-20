---
title:  Flintlock Home
layout: home
nav_order: 1
---

# Flintlock District Communitiess
![Flintlock District Community Map](assets/images/flintlock-map.jpg)

[Join the Council Mailing List](https://lp.constantcontactpages.com/sl/zZ8QRqh){: .btn .btn-green } 

## Important Monthly Events 

|Event| When & Where | Contact |
|:-------------|:------------------|:------|
|**Scouter's Roundtable**| 2nd Wednesday of the month 7-9pm @ [Marshall Simonds Middle School](https://maps.app.goo.gl/CK8aEn8KGiVSkJ8D8)| |
|**District Committee**| 1st Wednesday of the month 7:30-9pm @ [Bedford American Legion](https://maps.app.goo.gl/DKGcygk22jroEfBo7) | [Peter Rici](mailto:riccistuff@verizon.net)|
|**Eagle Board of Review** | 1st Monday of the month 7-8:30pm @ [St. Theresa's Parish](https://maps.app.goo.gl/jNkYBMrTedvgVRDC7) |  [Contact Flintlock Eagle Coordinator](mailto:fl.eagle.coordinator@gmail.com)|
|**Eagle Board of Review** | 3rd Thursday of the month 7:30-9pm @ [St. Brigid's Parish](https://maps.app.goo.gl/y9o9X4zvdmCSjNJF7)  |  [Contact Flintlock Eagle Coordinator](mailto:fl.eagle.coordinator@gmail.com)|
  

[Contact Peter Ricci for questions about District Events](mailto:riccistuff@verizon.net){: .btn .btn-green } 


## What's New from Flintlock District
<div>
  {% for post in site.posts %}
      <a href="{{ post.url }}">{{ post.date | date_to_long_string: "ordinal", "US" }}: {{ post.title }}</a>
      {{ post.excerpt }}
  {% endfor %}
</div>

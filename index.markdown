---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Faculty

{% for member in site.faculty %}
  <div class="faculty">
    <h3>{{ member.first_name }} {{ member.last_name }}</h3>

    <ul>
      <li>Email: {{ member.email }}</li>
      <li>Phone: {{ member.phone }}</li>
    </ul>

    {{ member.content | markdownify }}
  </div>
{% endfor %}

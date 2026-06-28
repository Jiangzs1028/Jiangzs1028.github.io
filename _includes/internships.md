<h2 id="internship-experience" style="margin: 2px 0px 10px;">Internship Experience</h2>

<div class="internships">

{% for item in site.data.internships.main %}

<div class="internship-row" style="margin: 0 0 24px;">
  {% if item.logo %}
  <div style="margin-bottom: 6px;">
    <img src="{{ item.logo }}" alt="{{ item.company }} logo" style="max-height: 46px; max-width: 300px; width: auto; height: auto;">
  </div>
  {% endif %}
  <div style="font-size: 1.05rem; font-weight: 600; color: #666; line-height: 1.45;">
    {{ item.time }}{% if item.description %}, {{ item.description }}{% endif %}
  </div>
</div>

{% endfor %}

</div>

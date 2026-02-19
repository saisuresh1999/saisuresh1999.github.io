<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative; padding-right: 15px; padding-left: 15px;">
    {% if link.conference_short %}
    <div style="margin-bottom: 6px;">
      <abbr class="badge">{{ link.conference_short }}</abbr>
    </div>
    {% endif %}
    {% if link.image %}
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1"
         style="width: 100%; height: auto; object-fit: contain; border-radius: 6px; display: block;">
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative; padding-right: 15px; padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em></div>
    <div class="links">
      {% if link.notes %}
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>

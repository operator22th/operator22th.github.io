<h2 id="experience" style="margin: 2px 0px -15px;">Experience</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.experience.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      {% if link.description %} 
      <div class="description">
      {{ link.description }}
      {% if link.time %} 
      <div class="time">
      {{ link.time }}
      </div>
      {% endif %}
      {% if link.language %} 
      <div class="language">
      <strong>Language: </strong>{{ link.language }}</div>
      {% endif %}
      </div>
    <div class="links">
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Lab Website</a>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>

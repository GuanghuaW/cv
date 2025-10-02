<div class="teaching">
  <ol class="teaching-list">
    {% for course in site.data.teaching %}
    <li>
      <div class="teaching-row">
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><strong>{{ course.title }}</strong></div>
          <div class="details">
            {{ course.role }}, {{ course.university }} ({{ course.term }})
          </div>
          {% if course.notes %}
            <div class="notes"><em>{{ course.notes }}</em></div>
          {% endif %}
          {% if course.link %}
            <a href="{{ course.link }}" target="_blank" style="font-size:12px;">Syllabus</a>
          {% endif %}
        </div>
      </div>
    </li>
    <br>
    {% endfor %}
  </ol>
</div>
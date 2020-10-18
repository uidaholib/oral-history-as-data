<div >
  <figure class="figure {{ include.class }} m-4">{% if include.link %}<a href="{{include.link}}" target="_blank">{%endif%}
    <img src="{{ include.img | prepend: '/images/' | absolute_url }}" class="figure-img img-fluid rounded border" alt="{{ include.alt }}">{% if include.link%}</a>{%endif%}
    <figcaption class="figure-caption">{{ include.caption }}</figcaption>
  </figure>
</div>
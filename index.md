- [guitarra](/assets/models/fender_stratocaster.usdz)
- [chair](/assets/models/chair_swan.usdz)
- [gramophone](/assets/models/gramophone.usdz)
- [teapot](/assets/models/teapot.usdz)
- [toy_biplane](/assets/models/toy_biplane.usdz)
- [toy_drummer](/assets/models/toy_drummer.usdz)


<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>
<model-viewer src="https://modelviewer.dev/shared-assets/models/Astronaut.glb" alt="A 3D model of an astronaut" auto-rotate camera-controls></model-viewer>
[ver em AR](/assets/models/astronauta/astronauta.usdz)

<ul>
  {% for product in site.products %}
    <li>
      <h2><a href="/assets/models/{{ product.name }}/{{ product.name }}.usdz">Ver em AR {{ product.name }}</a></h2>
      <h2><a href="{{ product.link }}">Comprar {{ product.name }}</a></h2>
      <h3>{{ product.description }}</h3>
      <p>{{ product.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>

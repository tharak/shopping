- [guitarra](/assets/models/fender_stratocaster.usdz)
- [chair](/assets/models/chair_swan.usdz)
- [gramophone](/assets/models/gramophone.usdz)
- [teapot](/assets/models/teapot.usdz)
- [toy_biplane](/assets/models/toy_biplane.usdz)
- [toy_drummer](/assets/models/toy_drummer.usdz)


<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>
<model-viewer src="https://modelviewer.dev/shared-assets/models/Astronaut.glb" alt="A 3D model of an astronaut" auto-rotate camera-controls></model-viewer>

<table>
  {% for product in site.products %}
  <tr>
    <td><a href="assets/models/{{ product.usdz }}">Ver em AR</a></td>
    <td><a href="{{ product.link }}">Comprar {{ product.name }}</a></td>
    <td>{{ product.description }}</td>
    <td><p>{{ product.content | markdownify }}</p></td>
  </tr>
  {% endfor %}
</table>

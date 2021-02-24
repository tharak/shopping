- [guitarra](/assets/models/fender_stratocaster.usdz)
- [chair](/assets/models/chair_swan.usdz)
- [gramophone](/assets/models/gramophone.usdz)
- [teapot](/assets/models/teapot.usdz)
- [toy_biplane](/assets/models/toy_biplane.usdz)
- [toy_drummer](/assets/models/toy_drummer.usdz)

<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

<table>
  {% for product in site.products %}
  <tr>
    <td>
    <model-viewer alt="{{ product.description }}" src="assets/models/{{ product.glb }}" ios-src="assets/models/{{ product.usdz }}" auto-rotate camera-controls magic-leap ar>    
    </td>
    <td><a href="{{ product.link }}">Comprar {{ product.name }}</a></td>
    <td>{{ product.description }}</td>
  </tr>
  {% endfor %}
</table>

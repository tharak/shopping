<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

<h2>Use nossos links e ajude o site!<h2>

<table>
  {% for product in site.products %}
  <tr>
    <td><model-viewer alt="{{ product.description }}" src="assets/models/{{ product.glb }}" ios-src="assets/models/{{ product.usdz }}#custom={{ product.banner }}" auto-rotate camera-controls magic-leap ar /></td>
    <td><a href="{{ product.link }}">Comprar {{ product.name }}</a></td>
    <td>{{ product.description }}</td>
  </tr>
  {% endfor %}
</table>

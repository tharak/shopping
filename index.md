<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

<h2>Use nossos links e ajude o site!<h2>


  {% for product in site.products %}
  <table style="width:100%">
    <tr><td><model-viewer alt="{{ product.description }}" src="assets/models/{{ product.glb }}" ios-src="assets/models/{{ product.usdz }}#custom=https://tharak.github.io/shopping/banners/{{ product.banner }}" auto-rotate camera-controls magic-leap ar /></td></tr>
    <tr><td><a href="{{ product.link }}">Comprar {{ product.name }}</a></td></tr>
    <tr><td>{{ product.description }}</td></tr>
  </table>
  {% endfor %}

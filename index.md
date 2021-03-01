<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">

<h2>Use nossos links e ajude o site!<h2>

<table style="width:100%">
  {% for product in site.products %}
  <tr>
    <td><model-viewer alt="{{ product.description }}" src="assets/models/{{ product.glb }}" ios-src="assets/models/{{ product.usdz }}#custom=https://tharak.github.io/shopping/banners/{{ product.banner }}" auto-rotate camera-controls magic-leap ar /></td>
    <td><a href="{{ product.link }}"> 
      <i class="material-icons" style="font-size:60px;color:lightblue;text-shadow:2px 2px 4px #000000;">shopping_cart</i>
      </a></td>
  </tr>
  {% endfor %}
</table>

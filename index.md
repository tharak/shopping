<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

<table style="width:100%">
  {% for product in site.products %}
  <tr>
    <td><model-viewer alt="{{ product.name }}" src="assets/models/{{ product.glb }}" ios-src="assets/models/{{ product.usdz }}" auto-rotate camera-controls magic-leap ar /></td>
    <td><a href="{{ product.link }}"> 
      <i class="material-icons" style="font-size:60px;color:lightblue;text-shadow:2px 2px 4px #000000;">shopping_cart</i>
      </a></td>
  </tr>
  {% endfor %}

  <tr>
    <td><model-viewer alt="A 3D model of a damaged helmet" src="https://modelviewer.dev/shared-assets/models/glTF-Sample-Models/2.0/DamagedHelmet/glTF/DamagedHelmet.gltf" ios-src="assets/models/{{ product.usdz }}" auto-rotate camera-controls magic-leap ar /></td>
    <td><a href="www.google.com"> 
      <i class="material-icons" style="font-size:60px;color:lightblue;text-shadow:2px 2px 4px #000000;">shopping_cart</i>
      </a></td>
  </tr>


  
</table>

<!DOCTYPE html>
<html>
<body>
  <input id="txt" placeholder="Digite uma palavra">
  <button onclick="conv()">Converter</button>
  <pre id="res"></pre>

  <script>
    function conv() {
      let t = document.getElementById("txt").value.split('').reverse();
      document.getElementById("res").textContent = t.map((l, i) => i % 2 == 0 ? l.toUpperCase() : l.toLowerCase()).join('\n');
    }
  </script>
</body>
</html>

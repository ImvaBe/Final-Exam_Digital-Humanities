<img id="fox-image" src="" alt="">

<script>
async function displayImage(){
    const response = await fetch('https://randomfox.ca/floof/');
    const data = await response.json();
    document.getElementById("fox-image").src = data.image;
  }
   
  displayImage();
  </script>
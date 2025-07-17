---
layout: default
title: Image Upscaler
---

# Welcome to My Image Upscaler

Upload your image below and get started.

<form id="uploadForm">
  <input type="file" id="upload" accept="image/*"><br><br>
  <img id="preview" style="max-width:400px;" />
</form>

<script>
  document.getElementById('upload').addEventListener('change', function(e) {
    const file = e.target.files[0];
    if (file) {
      document.getElementById('preview').src = URL.createObjectURL(file);
    }
  });
</script>

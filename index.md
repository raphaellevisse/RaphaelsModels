---
layout: default
title: Raphael's Models
---

# Image Upscaler


Let's stop it with sign ups or ads. Free, no quota, no suspicious downloads. AI needs to be for the people and not impossible to access through 1 billion terminal line instructions and docker installs on Github. Or another way to get your privacy.

This website is to give _easy_ access to state of the art quality. The easiest one is upsampling (2x-ing resolution). Just upload your image, click run and download your new image.

***

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


***

Work in progress. I need to figure out how to run inference fast and without costing me a rent.
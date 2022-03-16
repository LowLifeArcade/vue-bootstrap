<template>
  <footer class="footer p-4 m-0 bg-secondary">
    <div class="row d-flex justify-content-between">
      <div class="col-4">
        <div class="link">link</div>
        <div class="link">link</div>
        <div class="link">link</div>
      </div>
      <div class="col-4">
        <div class="link">link</div>
        <div class="link">link</div>
        <div class="link">link</div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent',
  props: {
    msg: String
  }
}

</script>
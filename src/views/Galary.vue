<template>
  <div class="about">
    <b-card
        :title="name"
        :img-src="img"
        img-alt="Image"
        img-top
        tag="article"
        style="max-width: 20rem;"
        class="mb-2"
      >
    </b-card>
  </div>
</template>
<script>
export default {
  props: ["name", "img","id","age","breed","category"],
  computed: {
    modalId() {
      return `modal-${this.id}`;
    }
  }
};
</script>

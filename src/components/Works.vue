<template>
  <section>
    <img src="@/assets/works/coffee&talk.png" alt="coffee&talk" />
    <img src="@/assets/works/opaoma.png" alt="coffee&talk" />
    <img src="@/assets/works/mr-wise.png" alt="coffee&talk" />

    <img src="@/assets/works/neuen-bazaar.png" alt="coffee&talk" />
    <img src="@/assets/works/kopenhagen-conchadeira.png" alt="coffee&talk" />
    <img src="@/assets/works/redx.png" alt="coffee&talk" />

    <img src="@/assets/works/redgroup.png" alt="coffee&talk" />
    <img src="@/assets/works/experience-day.png" alt="coffee&talk" />
    <img src="@/assets/works/redhouse.png" alt="coffee&talk" />
  </section>
</template>

<script>
export default {
  name: "Works",
};
</script>

<style scoped>
section {
  flex: none;
  order: 0;
  flex-grow: 0;

  margin: 100px 0 100px 0;
}
img {
  margin: 25px;
  width: 349px;
  height: 200px;

  filter: drop-shadow(0px 0px 8px rgba(0, 0, 0, 0.5));
  border-radius: 10px;
}
</style>

<template>
  <section id="about" class="container">
    <h1>About</h1>
    <div class="row gx-5">
      <figure class="col-md-6">
        <img src="../assets/images/profile.jpg" alt="" />
        <figcaption>About Michael Kwon</figcaption>
      </figure>
      <p class="col-md-6">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eveniet
        corporis libero magnam repellat, inventore voluptatem explicabo placeat
        maiores sunt recusandae laboriosam odit blanditiis nihil nobis. Nihil
        voluptates exercitationem fuga repudiandae!
      </p>
    </div>

    <article class="row mt-5">
      <h2>Skills</h2>
      <dl v-for="data in skills">
        <dt class="lead">{{ data.name }}</dt>
        <dd>
          <div class="progress" role="progressbar">
            <div class="progress-bar" :style="{ width: data.point }"></div>
          </div>
        </dd>
      </dl>
    </article>
  </section>
</template>
<script setup>
const skills = [
  { name: "HTML", point: "90%" },
  { name: "CSS", point: "80%" },
  { name: "JAVASCRIPT", point: "50%" },
  { name: "VUE", point: "75%" },
];
</script>
<style lnag="scss">
figure {
  img {
    width: 100%;
  }
}
</style>

<template>
  <Layout>
    <img class="greet-image" src="../../uploads/hello.svg" />

    <h2 class="mb-4">Khoirul Afandi</h2>
    <p>
      Hi, i'm Afandi. A passionate and fast learner PHP Developer with over 9+ years experience from Surabaya, Indonesia.
    </p>

    <h3 class="mt-5 mb-4">General Info</h3>
    <ul>
      <li>
        <b>Date Of Birth - </b> December 29, 1994
      </li>
      <li>
        <b>Address - </b> Surabaya
      </li>
      <li>
        <b>Email - </b> productive.afandi@gmail.com
      </li>
      <li>
        <b>Phone - </b> +62 838 3095 6015
      </li>
    </ul>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Gridsome starter bootstrap'
  }
}
</script>

<style>
.greet-image {
  display: block;
  margin: auto;
  width: 90%;
  max-width: 500px;
  padding-bottom: 50px;
}
</style>

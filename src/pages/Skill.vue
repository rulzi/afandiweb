<template>
  <Layout>
    <img class="about-image" src="../../uploads/content.svg" />
    <h3 class="mb-4">What I Can Do</h3>
    <ul>
      <li>
        <b>PHP - </b> I mostly use laravel for my project.
      </li>
      <li>
        <b>HTML/CSS - </b> have basic knowledge using this for implementation frontend. 
      </li>
      <li>
        <b>MySQL - </b> Using this for my Database, sometime with PostgreSQL.
      </li>
      <li>
        <b>GOLANG - </b> Use this in my office now for backend service.
      </li>
    </ul>

    <h3 class="mb-4">What I Can Build</h3>
    <ul>
      <li>
        <b>Profile Company - </b> Creating Web for your company.
      </li>
      <li>
        <b>Web Application - </b> Make your workflow offline goes to online. 
      </li>
      <li>
        <b>Web Travel - </b> Searching Flight on your own website.
      </li>
      <li>
        <b>Creating API - </b> Bridging Web for another web or apps.
      </li>
    </ul>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Skill'
  }
}
</script>

<style lang="scss" scoped>
.about-image {
  display: block;
  margin: auto;
  width: 90%;
  max-width: 500px;
  padding-bottom: 50px;
}
</style>

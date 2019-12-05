<template>
  <Layout>
    <div>
      <img class="contact-image mb-4" src="../../uploads/email.svg" />
      <div class="text-center">
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfYJDsPnHtkvyYu6Zvlmyz9oG6NTSUW5KousCjwdV2b55_zYQ/viewform?embedded=true" width="800" height="751" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
      </div>
    </div>
  </Layout>
</template>

<script>
  export default {
    metaInfo: {
      title: 'Contact'
    },
    data() {
      return {
        form: {
          name: '',
          email: '',
          message: '',
        },
      }
    },
    methods: {
      encode(data) {
        return Object.keys(data)
          .map(key => encodeURIComponent(key) + '=' + encodeURIComponent(data[key]))
          .join('&')
      },
      handleSubmit(e) {
        fetch('/', {
          method: 'POST',
          headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
          body: this.encode({
            'form-name': e.target.getAttribute('name'),
            ...this.form,
          }),
        })
        .then(() => this.$router.push('/success'))
        .catch(error => alert(error))
      }
    }
  }
</script>

<style scoped lang="scss">
.contact-image {
  display: block;
  margin: auto;
  width: 90%;
  max-width: 500px;
}
</style>

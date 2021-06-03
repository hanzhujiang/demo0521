<template>
  <div class="about">
    <h1>This is an about page</h1>
    <iframe :src="link" frameborder="0" style="padding: 0;width:100%;" height="500px"></iframe>
  </div>
</template>

<script>
export default {
components: {},
data() {
return {
  link:''
};
},
computed: {},
watch: {},
methods: {

},
created() {
this.link='https://survey-staging.arcnet.com.au/#/shortsurvey?originatortype=2&originatorid=1648050067&a=1810716428&p=1173116306&ref='+sessionStorage.getItem('ref')+'&iframe=1'
// this.link='http://localhost:8080/#/shortsurvey?originatortype=2&originatorid=1&p=937157695&ref=1'+sessionStorage.getItem('ref')+'&iframe=1'
console.log('link',this.link);

},
mounted() {

},
beforeCreate() {}, 
beforeMount() {}, 
beforeUpdate() {}, 
updated() {}, 
beforeDestroy() {}, 
destroyed() {}, 
activated() {}, 
}
</script>
<style lang='scss' scoped>
</style>
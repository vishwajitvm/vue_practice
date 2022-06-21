<template>
  <div>
    <div v-html="tag"></div>
    <div v-html="tag2"></div>
  </div>
</template>

<script>
export default {
    name: 'HtmlBindingCompo',
    data() {
        return {
            tag:"<h1>this is dynamic Tag</h1>",
            tag2:"<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis ratione quis quod qui recusandae facere odit atque sunt aliquid voluptate nulla non at, laborum doloremque deserunt beatae. Corporis quis ullam quam explicabo asperiores totam nam, voluptas deserunt temporibus necessitatibus, ea similique nisi aperiam quas cum quod. Illum architecto voluptatem eius exercitationem nulla accusamus temporibus. Quae sapiente ipsum perspiciatis esse repudiandae eligendi quod nulla veritatis temporibus vel ad repellendus, delectus vitae inventore quos nobis neque. Est inventore cum consequatur nisi voluptates consectetur et culpa aliquam. Quaerat, autem nulla molestiae laborum voluptate cum omnis fuga esse ratione odit quam mollitia iure alias accusantium. Voluptates natus vitae optio similique reprehenderit sunt minus eligendi. Accusamus natus explicabo perspiciatis reiciendis. Animi laudantium iste necessitatibus rem aperiam totam eaque nulla laborum illo delectus repellendus dolor possimus voluptatibus asperiores iusto provident, ut libero aut in? Omnis, molestias? Quasi, doloribus facere magni iste eligendi asperiores ex distinctio tempora</p>"
        }
    }
}
</script>

<style>
h1{
    color: white;
}
p{
    color:yellow
}
</style>
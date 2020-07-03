<template>
    <div>
        <ul id="example-1">
            <li v-for="item in items" :key="item.message">
                {{ item.message }}
            </li>
        </ul>
        <Button type="primary" @click.native="greet">Greet</Button>
    </div>
</template>

<script>
    export default {
        name: 'page2',
        data: function () {
            return {
                items: [
                    {message: 'Page2----A'},
                    {message: 'Page2----B'}
                ]
            }
        },
        methods: {
            greet: function (event) {
                alert('Hello ' + this.name + '!')
                if (event) {
                    // // 字符串
                    // this.$router.push('/home/first')
                    // // 对象
                    // this.$router.push({ path: '/home/first' })
                    // // 命名的路由
                    // this.$router.push({ name: 'home', params: { userId: wise }})
                    this.$router.push('/page1')
                    alert(event.target.tagName)
                }
            }
        }
    }
</script>

<style scoped>

</style>

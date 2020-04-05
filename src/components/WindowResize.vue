<template>
    <div>
        
    </div>
</template>

<script>
    export default {
        props: ['value'],
        name: 'VueWindowResize',
        computed: {
            window: {
                get() {
                    return this.value;
                },
                set(val) {
                    this.$emit('input', val)
                }
            }
        },
        created() {
            window.addEventListener('resize', this.handleResize);
            this.handleResize();
        },
        destroyed() {
            window.removeEventListener('resize', this.handleResize);
        },
        methods: {
            handleResize() {
                this.window.width = window.innerWidth;
                this.window.height = window.innerHeight;
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>
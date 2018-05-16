<template>
    <div>
        <p>
            foo is {{ foo }}
        </p>
    </div>
</template>

<script>
    export default {
        name: 'foo-1',
        data() {
            return {
                foo: 'bar'
            }
        }
    };
</script>

<style scoped>

</style>

<template>
    <div>
        <h2>This is user's {{$route.params.id}}</h2>
    </div>
</template>
<script>
export default {
    validate(context) {
        return /^\d+$/.test(context.params.id)
    }
}
</script>

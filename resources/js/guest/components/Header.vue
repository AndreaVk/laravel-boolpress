<template>
    <header>
        <h2>Header</h2>
        <a href="/admin/home">Area Riservata</a>
        <nav>
            <li>
                <router-link :to="{ name: 'home' }">Home</router-link>
            </li>
            <li>
                <router-link :to="{ name: 'about' }">Chi siamo</router-link>
            </li>
        </nav>
    </header>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style>

</style>
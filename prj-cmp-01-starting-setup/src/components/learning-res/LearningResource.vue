<template>
    <li>
        <base-card>
            <header>
                <h3>{{ title }}</h3>
                <base-button :mode="type">Delete</base-button>
            </header>
        <p>{{ description }}</p>
        <nav>
            <a :href="link">Open Web Res</a>
        </nav>
        </base-card>
    </li>
</template>

<script>
export default {
    props: ['title', 'description','link']
}
</script>

<style scoped>
li {
    margin: auto;
    max-width: 40rem;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

p {
    margin: 0.5rem 0;
}

a {
    text-decoration: none;
    color: #ce5c00;
}

a:hover,
a:active {
    color: #c89300;
}
</style>
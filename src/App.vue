<template>
    <section>
        <h2>My Friends</h2>
            <ul>
                <li></li>
            </ul>
    </section>
</template>

<script>
export default {
    data() {
        return {
            friends: [
                {
                    id: 'maria',
                    name: 'Maria Colina',
                    phone: '655 555 555',
                    email: 'maria.colina@localhost.com'
                },
                {
                    id: 'pep',
                    name: 'Pep Capdepera',
                    phone: '655 555 555',
                    email: 'pep.capdepera@localhost.com'
                }
            ]
        };
    },
    // methods: {},
    // computed: {}
};
</script>

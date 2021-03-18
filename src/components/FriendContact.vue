<template>
    <li>
        <h2>{{ name }}</h2>
        <button @click="toggleDetails">Show Details</button>
        <!-- <button @click="toggleDetails">{‌{ detailsAreVisible ? 'Hide' : 'Show' }} Details</button> -->
        <ul v-if="detailsAreVisible">
            <li><strong>Phone:</strong>{{ phoneNumber }}</li>
            <li><strong>Email:</strong>{{ emailAddress }}</li>
        </ul>
    </li>
</template>

<script>
export default {
    props: [
        'name',
        'phoneNumber',
        'emailAddress'
    ],
    data() {
        return {
            detailsAreVisible: false,
            friend: {
                    id: 'maria',
                    name: 'Maria Colina',
                    phone: '655 555 555',
                    email: 'maria.colina@localhost.com'
                },
        };
    },
    methods: {
        toggleDetails() {
            this.detailsAreVisible = !this.detailsAreVisible;
        }
    }
};
</script>

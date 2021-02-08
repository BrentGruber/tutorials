<template>
    <div id="employee-form">
        <form @submit.prevent="handleSubmit">
            <label>Employee name</label>
            <input type="text" />
            <label>Employee Email</label>
            <input type="text" />
            <button>Add Employee</button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'employee-form',
    data() {
        return {
            employee: {
                name: '',
                email: '',
            },
        }
    },
    methods: {
        handleSubmit() {
            console.log('testing handleSubmit')
            this.$emit('add:employee', this.employee)
        }
    }
}
</script>

<style scoped>
  form {
    margin-bottom: 2rem;
  }

</style>
<template>
    <div id="employee-form">
        <form>
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
}
</script>

<style scoped>
  form {
    margin-bottom: 2rem;
  }

  button {
    background: #009435;
    border: 1px solid #009435;
  }

  .small-container {
    max-width: 680px;
  }

</style>
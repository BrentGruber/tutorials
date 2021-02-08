<template>
    <div id="employee-table">
        <table>
            <thead>
                <tr>
                    <th>Employee Id</th>
                    <th>Employee Name</th> 
                    <th>Employee Email</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="employee in employees" :key="employee.id">
                    <td>{{ employee.id }}</td>
                    <td>{{ employee.name }}</td>
                    <td>{{ employee.email }}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    name: 'employee-table',
    props: {
        employees: Array,
    },
}
</script>

<style scoped>
</style>
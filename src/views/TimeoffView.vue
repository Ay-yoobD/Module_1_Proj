<template>
  <div>
    <h1>Leave Request Form</h1>
    <div class="form-container">
      <form @submit.prevent="submitForm">

        <label for="name">Name:</label>
        <input type="text" id="name" v-model="form.name" required>

        <label for="date">Date:</label>
        <input type="date" id="date" v-model="form.date" required />

        <label for="type">Type:</label>
        <select id="type" v-model="form.type" required>
          <option selected disabled hidden value="">Please choose...</option>
          <option>Sick leave</option>
          <option>Annual leave</option>
          <option>Maternity leave</option>
          <option>Parental leave</option>
          <option>Bereavement</option>
          <option>Unpaid leave</option>
          <option>Study leave</option>
        </select>

        <label for="reason">Reason:</label>
        <textarea id="reason" v-model="form.reason" required></textarea>

        <button type="submit">Request</button>
      </form>

      <div v-if="leaveRequests.length" class="requests-list">
        <h2>Leave Requests</h2>
        <table>
          <thead>
            <tr>
              <th>Name</th>
              <th>Date</th>
              <th>Type</th>
              <th>Reason</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="(request, index) in leaveRequests" :key="index">

              <td>{{ request.name }}</td>
              <td>{{ request.date }}</td>
              <td>{{ request.type }}</td>
              <td>{{ request.reason }}</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TimeOffView',
  data() {
    return {
      form: {
        date: '',
        type: '',
        reason: ''
      },
      leaveRequests: []
    }
  },
  methods: {
    submitForm() {
      // Add a copy of the form data to leaveRequests array
      this.leaveRequests.push({ ...this.form })

      alert('Leave request submitted successfully!')

      // Reset form
      this.form.date = ''
      this.form.type = ''
      this.form.reason = ''
    }
  }
}
</script>

<style scoped>
* {
  font-family: "Lato", 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  color: #0f0f0f;
}

h1 {
  text-align: center;
}

form {
  width: 400px;
  border: 1px solid #0f0f0f;
  border-radius: 5px;
  margin: 0 auto;
  color: #0f0f0f;
  padding: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}

label {
  display: block;
  width: 95%;
  padding-bottom: 3px;
}

input,
select,
textarea {
  width: 99%;
  margin-bottom: 10px;
  padding: 5px;
  font-size: 14px;
  border: 1px solid #ccc;
  border-radius: 3px;
  box-sizing: border-box;
}

button {
  display: block;
  width: 100%;
  letter-spacing: 0.5px;
  background-color: white;
  border: 1px solid #0f0f0f;
  padding: 8px 0;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.3s, color 0.3s;
}

button:hover {
  background-color: #0C2C4A;
  color: #fff;
  border: 1px solid #0f0f0f;
}

.form-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  min-height: 100vh;
  padding-top: 50px;
  box-sizing: border-box;
}

/* Leave requests table styling */
.requests-list {
  margin-top: 30px;
  width: 400px;
}

.requests-list h2 {
  margin-bottom: 10px;
  text-align: center;
}

.requests-list table {
  width: 100%;
  border-collapse: collapse;
  box-shadow: rgba(0, 0, 0, 0.1) 0px 2px 4px;
}

.requests-list th,
.requests-list td {
  border: 1px solid #ccc;
  padding: 8px;
  text-align: left;
}

.requests-list th {
  background-color: #f4f6fb;
}
</style>

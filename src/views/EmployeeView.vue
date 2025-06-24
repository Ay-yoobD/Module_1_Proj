<template>
  <div class="container mt-4">
    <h2 class="mb-4">Employees</h2>
    <table class="table table-striped table-bordered">
      <thead class="table-dark">
        <tr>
          <th scope="col">#</th>
          <th scope="col">Name</th>
          <th scope="col">Position</th>
          <th scope="col">Department</th>
          <th scope="col">salary</th>
          <th scope="col">Employment-history</th>
          <th scope="col">Contact details</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="emp in employees" :key="emp.id">
          <th scope="row">{{ emp.id }}</th>
          <td>{{ emp.name }}</td>
          <td>{{ emp.position }}</td>
          <td>{{ emp.department }}</td>
          <td>{{ emp.salary }}</td>
          <td>{{ emp.employmentHistory }}</td>
          <td>{{ emp.contact }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      employees: [
        {
          id: 1,
          name: "Ay-yoob Dawood",
          position: "Software Engineer",
          department: "Development",
          salary: 70000,
          employmentHistory: "Joined in 2015, promoted to Senior in 2018",
          contact: "Ayoob2322dawood@moderntech.com"
        },
        {
          id: 2,
          name: "Laila Abdurahman",
          position: "HR Manager",
          department: "HR",
          salary: 80000,
          employmentHistory: "Joined in 2013, promoted to Senior Manager in 2017",
          contact: "lailaabdurahman@moderntech.com"
        },
        {
          id: 3,
          name: "Zayaan Salie",
          position: "Quality Analyst",
          department: "QA",
          salary: 55000,
          employmentHistory: "Joined in 2018",
          contact: "zayaansalie@moderntech.com"
        },
        {
          id: 4,
          name: "Kauthar Naidoo",
          position: "Sales Representative",
          department: "Sales",
          salary: 60000,
          employmentHistory: "Joined in 2020",
          contact: "kauthar.naidoo@moderntech.com"
        },
        {
          id: 5,
          name: "zubair Davids",
          position: "Marketing Specialist",
          department: "Marketing",
          salary: 58000,
          employmentHistory: "Joined in 2019",
          contact: "zubair453@moderntech.com"
        },
        {
          id: 6,
          name: "Sipho Zulu",
          position: "UI/UX Designer",
          department: "Design",
          salary: 65000,
          employmentHistory: "Joined in 2016",
          contact: "sipho.zulu@moderntech.com"
        },
        {
          id: 7,
          name: "Natheerah Abdullah",
          position: "DevOps Engineer",
          department: "IT",
          salary: 72000,
          employmentHistory: "Joined in 2017",
          contact: "natheerah8909@moderntech.com"
        },
        {
          id: 8,
          name: "Farah thomas",
          position: "Content Strategist",
          department: "Marketing",
          salary: 56000,
          employmentHistory: "Joined in 2021",
          contact: "farah9081@moderntech.com"
        },
        {
          id: 9,
          name: "Daniel davis",
          position: "Accountant",
          department: "Finance",
          salary: 62000,
          employmentHistory: "Joined in 2018",
          contact: "Daniel2345@moderntech.com"
        },
        {
          id: 10,
          name: "Fatima Patel",
          position: "Customer Support Lead",
          department: "Support",
          salary: 58000,
          employmentHistory: "Joined in 2016",
          contact: "fatima.patel@moderntech.com"
        }
      ]
    };
  }
};
</script>

<style scoped>
.container {
  background: #ffffff;
  border-radius: 12px;
  box-shadow: 0 1px 16px rgba(46, 143, 240, 0.1);
  padding: 32px;
}

table {
  border-collapse: collapse;
}

th, td {
  text-align: left;
  padding: 10px 8px;
  font-size: 1rem;
}

thead {
  background-color: #3794f1;
  color: white;
}
</style>

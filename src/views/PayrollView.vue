<template>
    <div class="MainPayRoll">
        <header class="PayRollHead">
            <h2 class=" p-3 fw-bold">Payroll & Payslip management:</h2>
        </header>

        <main class="PayrollBody">
            <div class="container-xl ImageContain">
                <figure class="figure PayImage">
                    <img src="../assets/Meter.png" class="figure-img img-fluid rounded" alt="...">
                    <figcaption class="figure-caption">Total Number of Deductions severity</figcaption>
                </figure>

                <figure class="figure PayImage">
                    <img src="../assets/DonutChart.png" class="figure-img img-fluid rounded" alt="...">
                    <figcaption class="figure-caption">Total Paid Takeaway Salaries vs Not Paid</figcaption>
                </figure>

                <figure class="figure PayImage">
                    <img src="../assets/IncreasingGraph.png" class="figure-img img-fluid rounded" alt="...">
                    <figcaption class="figure-caption">Increasing number of ModernTech employees</figcaption>
                </figure>


            </div>

            <div class="container-xl">
                <hr style=" color: #2d5652; ">

                <div class="Title display-4 fw-bold">
                    <p>Payslip audit:</p>

                </div>
                <hr style=" color: #2d5652;">

                <section id="intro">
                    <div class="container-lg">
                        <div class="row justify-content-center align-items-center">
                            <div class="col-md-5 text-center text-md-start">
                                <div class="PayManageBody">
                                    <div class="info-card">
                                        <h3>Employee Salary & Payroll information:</h3>
                                        <dl class="student-info">
                                            <dt>Employee ID :</dt>
                                            <dd>Hello</dd>

                                            <dt>Hours employee worked::</dt>
                                            <dd>Hello</dd>

                                            <dt>Amount of deductions:</dt>
                                            <dd>Hello</dd>

                                            <dt>Final Salary after deductions:</dt>
                                            <dd>Hello</dd>
                                        </dl>
                                    </div>

                                </div>

                            </div>

                            <div class="col-md-5 text-center ">
                                <select name="EmployeeSelect" id="cmbEmployeeSelect" placeholder="Select Employee">
                                    <option value="" disabled selected hidden>Select Employee</option>
                                    <option value="volvo">Volvo</option>
                                    <option value="saab">Saab</option>
                                    <option value="mercedes">Mercedes</option>
                                    <option value="audi">Audi</option>
                                </select>
                                <br>
                                <button class="DeductionBtn">Show all deduction full details</button>

                                <p>
                                    <button class="DetailedPayBtn">Calculate & Display full payslip details</button>
                                    <button class="PrintPayBtn">Create Digital Payslip (PDF)</button>
                                </p>
                            </div>

                        </div>
                    </div>
                </section>

            </div>

        </main>

    </div>

</template>

<script>
export default {

}
</script>

<style>
.MainPayRoll {
    overflow-x: visible;
    font-family: Baskerville;
    background: rgb(255, 255, 255);
    min-height: 100vh;
}

.PayRollHead {
    background-color: #93d1cb;
    padding: 1rem 2rem 1rem 70px;
    margin: -1.5rem -1.5rem 1.5rem -1.5rem;
    box-shadow: 0 4px 4px rgba(147, 209, 203, 0.447);
    min-height: 70px;
    display: flex;
    align-items: center;

}

.PayRollHead h2 {
    margin: 0;
    font-size: 2.75rem;
    color: #2c3e50;
}

/* Ensures page content doesn't overlap */
.PayrollBody {
    padding-top: 1rem;
}


.PayImage {
    width: 350px;
    margin: 0px 30px;


}

.ImageContain {
    margin-top: 50px;
    margin-bottom: 50px;
}

.PayImage figcaption {
    color: #2c3e50;
    font-size: 18px;

}

.Title {
    margin: 15px;
    padding: 5px;
}

.DeductionBtn{
    margin: 40px;
    width: 500px;
    text-align: center;
    border-radius: 5px;
    border: #2d5652 solid 3px;
    box-shadow: #e2a54d 3px 3px;
    background: #93d1cb;
    padding: 7px 5px;
    transition: background 0.3s ease;
    transition: box-shadow 0.2s ease;
    transition: transform 0.3s ease;
    font-size: 18px;

}

.DeductionBtn:hover{
    background: #e2a54d;
    box-shadow: none;
    transform: scale(1.026);
}

.DetailedPayBtn{
    width: 160px;
    margin-right: 40px;
    padding: 10px 40px 10px 40px;
    text-align: center;
}

.PrintPayBtn{
    width: 160px;
    margin-right: 40px;
    padding: 10px 40px 10px 40px;
    text-align: center;
}


</style>
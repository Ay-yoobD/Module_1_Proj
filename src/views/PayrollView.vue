<template>
    <div class="MainPayRoll">
        <header class="PayRollHead">
            <h2>Payroll & Payslip management</h2>
        </header>

        <body class="PayrollBody">
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

                            <div class="col-md-5 text-center d-none d-md-block">
                                <button>hello</button><br>
                                <button>hello1</button>
                                <p><button>hello3</button> <button>hello4</button></p>
                            </div>

                        </div>
                    </div>
                </section>

            </div>

        </body>

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
}

.PayRollHead {
    background-color: rgb(147, 209, 203);
    padding: 1rem 2rem 1rem 70px;
    margin: -1.5rem -1.5rem 1.5rem -1.5rem;
    box-shadow: 0 4px 4px rgba(147, 209, 203, 0.447);
    min-height: 70px;
    display: flex;
    align-items: center;
}

.PayRollHead h2 {
    margin: 0;
    font-size: 1.5rem;
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

.Title{
    margin: 15px;
    padding: 5px;
}
</style>
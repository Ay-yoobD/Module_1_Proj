<template>
    <div class="offcanvas offcanvas-start maincollapse" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel" style="width: 280px; min-height: 100vh;     background: linear-gradient(to bottom, #0c2c47 55%, #7ea1af 100%);">
        <div class="offcanvas-header">
            <a href="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-white text-decoration-none">
                <span class="fs-4">Site Navigation</span>
            </a>
            <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
            <div>
                <div id="sidebar" class="MainSideBar d-flex flex-column flex-shrink-0 text-white collapse show">

                    <ul class="InnerSideBar nav nav-pills flex-column mb-auto">
                        <li class="nav-item Links" data-bs-dismiss="offcanvas">
                            <router-link to="/" class="nav-link text-info" aria-current="page">
                                Home
                            </router-link>
                        </li>
                        <hr>
                        <li class="Links" data-bs-dismiss="offcanvas">
                            <router-link to="/employees" class="nav-link text-white">
                                Employee Dashboard
                            </router-link>
                        </li>
                        <hr>
                        <li class="Links" data-bs-dismiss="offcanvas">
                            <router-link to="/payroll" class="nav-link text-white">
                                Payroll Regulation
                            </router-link>
                        </li>
                        <hr>
                        <li class="Links" data-bs-dismiss="offcanvas">
                            <router-link to="/timeoff" class="nav-link text-white">
                                Timeoff Requests
                            </router-link>
                        </li>
                        <hr>
                        <li class="Links" data-bs-dismiss="offcanvas">
                            <router-link to="/review" class="nav-link text-white">
                                Performance Reviews
                            </router-link>
                        </li>
                    </ul>
                    
                    <!-- <hr class="hrNav"> -->

                </div>
            </div>

        </div>
                            <div class="dropdown offcanvas-footer p-3">
                        <a href="#" class="d-flex align-items-center text-white text-decoration-none dropdown-toggle"
                            id="dropdownUser1" data-bs-toggle="dropdown" aria-expanded="false">
                            <img src="https://github.com/mdo.png" alt="" width="32" height="32"
                                class="rounded-circle me-2">
                            <strong>mdo</strong>
                        </a>
                        <ul class="dropdown-menu dropdown-menu-dark text-small shadow" aria-labelledby="dropdownUser1">
                            <li><a class="dropdown-item" href="#">New project...</a></li>
                            <li><a class="dropdown-item" href="#">Settings</a></li>
                            <li><a class="dropdown-item" href="#">Profile</a></li>
                            <li>
                                <hr class="dropdown-divider">
                            </li>
                            <li><a class="dropdown-item" href="#">Sign out</a></li>
                        </ul>
                    </div>
    </div>

</template>

<script>
export default {

}
</script>

<style>
/* .MainSideBar {
    min-height: 100vh;
    background: linear-gradient(to bottom, #0c2c47 55%, #7ea1af 100%);
    border-right: #0b273e solid;

} */

.hrNav {
    color: #00070d;
}



</style>
<template>
    <nav class="navbar navbar-light fixed-top bg-white p-0 shadow">
        <a class="navbar-brand col-sm-3 col-md-2 mr-0" href="#">
            <div class="d-flex flex-column justify-content-center text-center">
                <img src="@/assets/avatar.svg" alt="" srcset="">
                <a class="nav-link dropdown-toggle" href="#" data-toggle="profile" aria-haspopup="true" aria-expanded="false">
                    Aisha Coutoure
                </a>
            </div>
        </a>
        <input class="d-none d-lg-block searchbar" type="text" placeholder="Search" aria-label="Search">
        <ul class="navbar-nav ml-0 ml-md-auto flex-row align-items-center">
            <li class="nav-item text-nowrap">
                <Toggle></Toggle>
            </li>
            <li class="nav-item text-nowrap">
                <img src="@/assets/notification.svg" alt="" srcset="">
            </li>
            <li class="nav-item text-nowrap dropdown">
                <a class="nav-link dropdown-toggle" href="#" data-toggle="profile" aria-haspopup="true" aria-expanded="false">
                    <img src="@/assets/avatar.svg" alt="" srcset="">
                </a>
                <div class="dropdown-menu dropdown-menu-right" aria-labelledby="profile">
                    <a class="dropdown-item active" href="/docs/4.1/">Latest (4.1.x)</a>
                    <a class="dropdown-item" href="https://getbootstrap.com/docs/4.0/">v4.0.0</a>
                    <div class="dropdown-divider"></div>
                    <a class="dropdown-item" href="https://v4-alpha.getbootstrap.com/">v4 Alpha 6</a>
                    <a class="dropdown-item" href="https://getbootstrap.com/docs/3.3/">v3.3.7</a>
                    <a class="dropdown-item" href="https://getbootstrap.com/2.3.2/">v2.3.2</a>
                </div>
            </li>
        </ul>
    </nav>
</template>

<script>
import Toggle from "@/components/Toggle.vue";
export default {
  name: "Navbar",
  components: {
    Toggle
  },
  mounted() {}
};
</script>

<style scoped>
.navbar-brand {
  padding-top: 0.2rem;
  padding-bottom: 0.2rem;
  font-size: 1rem;
  background-color: white;
}

.navbar-brand * {
  color: #0d1532;
}

.navbar .form-control {
  padding: 0.75rem 1rem;
  border-width: 0;
  border-radius: 0;
}

.searchbar {
  background-color: #ffffff;
  border: 1px solid #0d1532;
  border-radius: 3px;
  background: url("../assets/search.svg") no-repeat scroll 360px 8px;
  transition: ease 0.5s;
  width: 400px;
  display: block;
  height: calc(2.25rem + 2px);
  padding: 0.375rem 0.75rem;
  font-size: 1rem;
  line-height: 1.5;
  border-radius: 0.25rem;
  -webkit-transition: border-color 0.15s ease-in-out,
    -webkit-box-shadow 0.15s ease-in-out;
  transition: border-color 0.15s ease-in-out,
    -webkit-box-shadow 0.15s ease-in-out;
  transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
  transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out,
    -webkit-box-shadow 0.15s ease-in-out;
}

.searchbar:focus {
  outline: 0;
  border: 1px solid #0d1532;
  color: #495057;
  background-color: #fff;
  -webkit-box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
  box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
}

.nav-item {
  padding: 0 20px;
}
</style>
<template>
    <nav class="col-md-2 d-none d-md-block text-white sidebar">
        <div class="sidebar-sticky">
            <ul class="nav flex-column">
                <li class="nav-item">
                    <a class="nav-link active" href="#">
                        <font-awesome-icon icon="home" />
                        Home <span class="sr-only">(current)</span>
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <font-awesome-icon icon="wallet" />
                        Wallet
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <font-awesome-icon icon="power-off" />
                        Getting Started
                    </a>
                </li>
                <br>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                       <font-awesome-icon icon="list-ul" />
                        Plans
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                       <font-awesome-icon icon="money-bill-alt" />
                        Transactions
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <font-awesome-icon icon="credit-card" />
                        Payment Pages
                    </a>
                </li>
                <br>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                       <font-awesome-icon icon="users" />
                        Teams
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                       <font-awesome-icon icon="user" />
                        Customers
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <font-awesome-icon icon="rss-square" />
                       Subscriptions
                    </a>
                </li>
                <br>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                       <font-awesome-icon icon="terminal" />
                        Developers
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                       <font-awesome-icon icon="cog" />
                        Business Settings
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
  name: "Sidebar"
};
</script>

<style scoped>
.nav-item {
  transition: ease 0.2s;
}

.nav-link {
  color: white;
  transition: ease 0.2s;
}

.nav-item:hover {
  background: white;
}

.nav-link:hover {
  color: #0d1532;
}
.sidebar .nav-link.active:hover {
  color: #0d1532;
}
.sidebar {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  z-index: 100;
  /* Behind the navbar */
  padding: calc(84px + 0.2rem) 0 0;
  /* Height of navbar */
  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.1);
  background: #0d1532;
}

.sidebar-sticky {
  position: relative;
  top: 0;
  height: calc(100vh - (84px + 0.2rem));
  padding-top: 0.5rem;
  overflow-x: hidden;
  overflow-y: auto;
  /* Scrollable contents if viewport is shorter than content. */
}

@supports ((position: -webkit-sticky) or (position: sticky)) {
  .sidebar-sticky {
    position: -webkit-sticky;
    position: sticky;
  }
}

.sidebar .nav-link .feather {
  margin-right: 4px;
  color: #999;
}

.sidebar .nav-link.active {
  color: white;
}
.sidebar .nav-link.active::before {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 2px;
  background: white;
}

.sidebar .nav-link:hover .feather,
.sidebar .nav-link.active .feather {
  color: inherit;
}

.sidebar-heading {
  font-size: 0.75rem;
  text-transform: uppercase;
}

svg {
  margin: 0 20px;
}
</style>
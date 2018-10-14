<template>
  <div id="app">
    <Navbar></Navbar>
    <div class="container-fluid">
      <div class="row">
        <Sidebar></Sidebar>
        <main role="main" class="col-md-9 ml-sm-auto col-lg-10 px-4">
          <div class="d-flex justify-content-between align-items-center pt-3 py-2 mb-3 border-bottom col-12">
              <a class="nav-link dropdown-toggle">
                    <font-awesome-icon icon="filter" />
                    Date
                </a>
                <div class="col-2 d-flex flex-row text-center color-primary">
                  <a class="nav-link flex-column color-primary" href="#">
                    <font-awesome-icon icon="plus-square" size="1x"/>
                    <p class="mb-0">Add</p>
                  </a>
                  <a class="nav-link flex-column color-primary" href="#">
                    <font-awesome-icon icon="download" size="1x"/>
                    <p class="mb-0">Download</p>
                  </a>

                </div>
          </div>
          <div class="table-responsive">
            <table class="table table-sm">
              <thead>
                <tr>
                  <th></th>
                  <th>Name</th>
                  <th>Interval</th>
                  <th>Amount</th>
                  <th>Count</th>
                  <th>Description</th>
                  <th>Updated At</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
                <tr>
                  <td>Jane Doe</td>
                  <td>6</td>
                  <td>GHC 270</td>
                  <td>10</td>
                  <td>Lorem Ipsum</td>
                  <td>22/22/22</td>
                </tr>
              </tbody>
            </table>
          </div>
          <footer class="py-2">
            <div class="d-flex col-12 justify-content-end"><b>Powered By <br></b>
              <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iODQiIGhlaWdodD0iMjUiIHZpZXdCb3g9IjAgMCA4NCAyNSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4NCiAgICA8dGl0bGU+DQogICAgICAgIGF0bGFzX2xvZ28NCiAgICA8L3RpdGxlPg0KICAgIDxnIGZpbGwtcnVsZT0ibm9uemVybyIgZmlsbD0ibm9uZSI+DQogICAgICAgIDxwYXRoIGQ9Ik0yMC44NTggMTMuOTIyYTUuMDQ1IDUuMDQ1IDAgMCAwLTIuNzMtNy4wMDEgNS45MzUgNS45MzUgMCAwIDEtMS4yNzMgMi4yNTEgMi41MSAyLjUxIDAgMSAxLTEuOTEyLjM4NUE1LjA0MiA1LjA0MiAwIDEgMCA3LjQzMyA1LjhhNS44OSA1Ljg5IDAgMCAxIDIuNTg3LjA5MiAyLjUyIDIuNTIgMCAxIDEgLjk4NCAxLjM3MkEzLjk3NiAzLjk3NiAwIDAgMCA4LjUyIDYuNjFhNS4wNDIgNS4wNDIgMCAwIDAtMS43MjQgOS43NyAzLjA3IDMuMDcgMCAxIDEtMS45NDItLjA3MyA1Ljk4NCA1Ljk4NCAwIDAgMS0xLjY1OS0yLjA0NiA1LjYwMyA1LjYwMyAwIDEgMCA0LjU5OC0uMjA0IDIuNTIgMi41MiAwIDEgMSAzLjI0Ny0yLjQxOCAyLjU1IDIuNTUgMCAwIDEtMS41NTYgMi4zMzMgNi41NDcgNi41NDcgMCAwIDEgMS43NzQgMS45MDNjLjQ0Ny0uMjkuODQ1LS42NSAxLjE4LTEuMDY0YTUuMDQ1IDUuMDQ1IDAgMCAwIDUuODA0IDEuNTA5IDMuMDgyIDMuMDgyIDAgMSAxLTEuNjYyIDEuMjU2IDUuOTAyIDUuOTAyIDAgMCAxLTIuNTg2LS40OTJjLS4yMTEuNC0uNDMxIDEuNDM3LS40MzEgMi4xNzZhNS42MDMgNS42MDMgMCAxIDAgNy4yOTYtNS4zMzd6IiBmaWxsPSIjMjQ1MUNBIi8+DQogICAgICAgIDxwYXRoIGQ9Ik00Mi43MDEgMjAuNTQ2YS42OTguNjk4IDAgMCAxLS42NTUtLjQ4NCA3NC43ODcgNzQuNzg3IDAgMCAwLS41NTktMS42IDYwLjMxNSA2MC4zMTUgMCAwIDEtLjcxOC0yLjEwOWgtNy4yNTZjLS4yMzIuNzItLjQ2OCAxLjQyOC0uNzA4IDIuMTIzLS4xODQuNTMyLS4zNjYgMS4wNjItLjU0NSAxLjU4OWEuNjk3LjY5NyAwIDAgMS0uNjUuNDgxaC0xLjc3OGEuNzE4LjcxOCAwIDAgMS0uNjU1LS45NjNjLjUyNC0xLjUzMiAxLjAyNi0yLjk2OSAxLjUwNS00LjMxLjU3NS0xLjYxMSAxLjE0LTMuMTM3IDEuNjk2LTQuNTc4YTE2OC43MiAxNjguNzIgMCAwIDEgMS42NDYtNC4xMTUgMTM0Ljc2IDEzNC43NiAwIDAgMSAxLjYyMS0zLjcyLjIzMS4yMzEgMCAwIDEgLjIxLS4xNDNoMi42ODVhLjIzMS4yMzEgMCAwIDEgLjIxLjE0NCAxMzcuNzQ5IDEzNy43NDkgMCAwIDEgMy4yNyA3LjgzNGMuNTU0IDEuNDQgMS4xMjQgMi45NjYgMS43MSA0LjU3OC40ODYgMS4zNDEuOTkyIDIuNzc4IDEuNTE5IDQuMzFhLjcxOC43MTggMCAwIDEtLjY1Ni45NjNoLTEuODkyem0tNS4yNDEtMTMuNmEuMzQyLjM0MiAwIDAgMC0uNjQxIDBjLS4yOTguNzQtLjYyNSAxLjU4NS0uOTggMi41MzRhMTg2LjIyMyAxODYuMjIzIDAgMCAwLTEuNTI0IDQuMjQ0aDUuNjVjLS41My0xLjUyNi0xLjA0Mi0yLjk1LTEuNTM3LTQuMjctLjM1Ny0uOTUyLS42OC0xLjc4OC0uOTY4LTIuNTA5em0yOS44OTMtLjE5M2MuOTkyIDAgMS44MjYuMTI5IDIuNTAzLjM4Ni42MjMuMjIgMS4xOC41OTIgMS42MjQgMS4wOGE0LjEgNC4xIDAgMCAxIC44NjIgMS42ODVjLjE4LjcxLjI2NyAxLjQ0LjI2IDIuMTc0djcuNTU4YS43MTguNzE4IDAgMCAxLS41NzUuNzFjLS40MDguMDc3LS45MTYuMTYzLTEuNTI0LjI1N2EyMC42NTggMjAuNjU4IDAgMCAxLTMuMTYxLjIxOSA5LjE1IDkuMTUgMCAwIDEtMi4xMTItLjIzMSA0LjM5NSA0LjM5NSAwIDAgMS0xLjY0OC0uNzQ2IDMuNDg0IDMuNDg0IDAgMCAxLTEuMDY2LTEuMzM4IDQuNzgzIDQuNzgzIDAgMCAxLS4zODQtMi4wMzEgNC4wNDMgNC4wNDMgMCAwIDEgLjQzMS0xLjk1NmMuMjgyLS41Mi42ODYtLjk2NCAxLjE3Ny0xLjI5M2E0Ljk5NCA0Ljk5NCAwIDAgMSAxLjcyNC0uNzE4IDkuMzcyIDkuMzcyIDAgMCAxIDIuMDQ1LS4yMTkgOC45NiA4Ljk2IDAgMCAxIDIuMjA0LjI4M3YtLjUyMWE0LjE3NCA0LjE3NCAwIDAgMC0uMTI0LTEuMDI5IDIuMTY4IDIuMTY4IDAgMCAwLS40MzEtLjg2MiAyLjAzNiAyLjAzNiAwIDAgMC0uODE3LS41NzUgMy40MjQgMy40MjQgMCAwIDAtMS4yNzYtLjIwNSAxMC45MiAxMC45MiAwIDAgMC0xLjkwOC4xNTNjLS4yNTEuMDQ2LS40ODIuMDkzLS42OTMuMTQ0YS42OTUuNjk1IDAgMCAxLS44NC0uNTk1TDYzLjQ2NCA4YS43MTguNzE4IDAgMCAxIC41MTMtLjgxNWMuMjk2LS4wNzYuNjQ1LS4xNTIgMS4wNDctLjIyOWExMi41NyAxMi41NyAwIDAgMSAyLjMzLS4yMDJ6bS4yNDkgMTEuNTk5Yy43MDUuMDE4IDEuNDExLS4wMzQgMi4xMDYtLjE1NFYxNC43NWE2LjQ1NCA2LjQ1NCAwIDAgMC0xLjc1OS0uMjMxYy0uMzM2IDAtLjY3Mi4wMjYtMS4wMDUuMDc3YTMuMDQ1IDMuMDQ1IDAgMCAwLS45MTcuMjg4Yy0uMjY1LjEzLS40OTIuMzI4LS42NTYuNTc0YTEuNjYgMS42NiAwIDAgMC0uMjQ5LjkzOWMwIC43MzcuMjIzIDEuMjQ3LjY3IDEuNTMuNDQ2LjI4MiAxLjA1LjQyNSAxLjgxLjQyNnYtLjAwMXptLTEzLjUxMy42MzRhNi4zNzUgNi4zNzUgMCAwIDEtLjI0OC0xLjEyOC4xNTIuMTUyIDAgMCAwLS4yMDUtLjEyOGMtLjIyMi4wODItLjQ5Ni4xNy0uODIxLjI2M2E1LjMgNS4zIDAgMCAxLTEuNDUuMThjLS43OTMgMC0xLjM1NS0uMjMyLTEuNjg1LS42OTUtLjMzLS40NjItLjQ5Ni0xLjIzNC0uNDk2LTIuMzE0di00Ljg4NWgzLjQ0OFY4LjA0NmEuMzQ4LjM0OCAwIDAgMC0uMzMzLS4zNmgtMy4xMTV2LTMuMzVhLjIzNi4yMzYgMCAwIDAtLjIzMS0uMjRsLTIuNTM1LjM5MWEuMjM2LjIzNiAwIDAgMC0uMjMxLjI0VjE1LjE5Yy0uMDEuNzk4LjA2NCAxLjU5Ni4yMjEgMi4zNzkuMTI1LjY0LjM4NyAxLjI0NS43NjkgMS43NzQuMzguNTAyLjg5Ljg4OSAxLjQ3NCAxLjEyLjYyLjI1NiAxLjM5Mi4zODUgMi4zMTYuMzg2Ljc2IDAgMS40MDctLjE0NCAxLjk4My0uMjQ0LjM3Mi0uMDYzIDEuMDI3LS4yNDQgMS40MzYtLjM2NGEuMTkuMTkgMCAwIDAgLjExLS4yNzUgNC44MjkgNC44MjkgMCAwIDEtLjQwNy0uOTh6bTYuNTY4LS44ODNhLjE0NC4xNDQgMCAwIDAtLjE3NC0uMTA2IDIuNDcgMi40NyAwIDAgMS0xLjA4LjAxNiAxLjgyIDEuODIgMCAwIDEtLjYwNi0uNDExIDEuNTQgMS41NCAwIDAgMS0uMzEtLjY1NSA0LjQwMiA0LjQwMiAwIDAgMS0uMDg2LS45NTFWMi45NTZhLjIzNi4yMzYgMCAwIDAtLjIzMS0uMjRsLTIuNTM2LjM4N2EuMjM2LjIzNiAwIDAgMC0uMjMyLjI0djEzLjIzNWE2LjkwOCA2LjkwOCAwIDAgMCAuMjEyIDEuNzg3Yy4xMjQuNDk0LjM3Ni45NDYuNzMgMS4zMTIuMzk2LjM3OC44NzYuNjU2IDEuNC44MS41MjguMTYyIDIuNjQ0LjQ5NCAzLjczNi0uMTgyYS4xMy4xMyAwIDAgMCAuMDM0LS4xOTEgNC4xOTggNC4xOTggMCAwIDEtLjY4Mi0xLjM3NyA1Ljg5IDUuODkgMCAwIDEtLjE3NS0uNjM0em0xMy41MzggMS45MjZhLjM1LjM1IDAgMCAwIC4yODguMzU3YzEuMjQ0LjE4OSAzLjY3LjQ2OSA1LjI2NC4yNjIgMi4zMjMtLjMwMiA0LjMxLTEuNTYyIDQuMDA3LTQuNTMtLjMzNy0yLjk3Ni0yLjMwNC0zLjQ3NC00LjU4Ny0zLjk2My0yLjI1My0uNDMtMi4yOC0xLjQyNy0xLjg4MS0yLjAyMy4yMS0uMjcuNDk5LS40NjcuODI2LS41NjYuNDMtLjE0NS44ODItLjIxNSAxLjMzNi0uMjA1LjY0LjAyMyAxLjI3Ni4xMDQgMS45MDEuMjQxLjI0Ny4wNDguNDc1LjA5OS42ODMuMTUyYS42OTQuNjk0IDAgMCAwIC44NjItLjU3NGwuMTc1LTEuMDg0YS43MTguNzE4IDAgMCAwLS41MDYtLjgxOWMtLjI5Ni0uMDgtLjY0NS0uMTYyLTEuMDQ3LS4yNDRhMTIuNTczIDEyLjU3MyAwIDAgMC0yLjMyNi0uMjQxYy0uOTkyLS4wMTYtMS44MjguMS0yLjUwOS4zNDdhMy45OCAzLjk4IDAgMCAwLTEuNjQgMS4wNSA0LjE1IDQuMTUgMCAwIDAtLjg5MiAxLjY3MmMtLjU1NyAxLjgxOS40OTkgNC4yMyAyLjYxOCA0LjY1NiAyLjEyLjQyNyA0LjAzLjIyIDMuOTI4IDIuMDUtLjEyNSAxLjc4LTQuNTk3IDEuMTk3LTYuMzEuODg0YS4xMjIuMTIyIDAgMCAwLS4xNDQuMTJsLS4wNDYgMi40NTh6IiBmaWxsPSIjMEUwRjIyIi8+DQogICAgPC9nPg0KPC9zdmc+DQo=" alt="" srcset="">
            </div>
          </footer>
        </main>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";
export default {
  name: "app",
  components: {
    Navbar,
    Sidebar
  }
};
</script>

<style>
[role="main"] {
  padding-top: calc(84px + 0.2rem); /* Space for fixed navbar */
}
body {
  font-size: 0.875rem;
}

.footer {
}
.feather {
  width: 16px;
  height: 16px;
  vertical-align: text-bottom;
}

.color-primary {
  color: #0d1532;
  transition: ease 0.2s;
}
.color-primary:hover {
  color: #0d1532a4;
}
.table-responsive {
  max-height: 500px;
}
tbody tr {
  transition: ease 0.5s;
  border-left: solid 5px transparent;
  padding: 20px;
}

tbody tr:hover {
  background: #cdcfd6;
  border-left-color: #0d1532;
}

tbody tr::before {
  position: absolute;
  height: 24px;
  top: 0;
  width: 5px;
  background: transparent;
  content: "";
  transition: 0.5s ease;
}

tr {
  position: relative;
}
tbody tr:hover {
  background: #cdcfd6;
}

tbody tr::before:hover {
  background: #0d1532;
}

.table td,
.table th {
  padding: 1rem 0px !important;
  text-align: center;
}

thead {
  background: #0d1532;
  color: white;
  text-align: center;
}

::-webkit-scrollbar {
  width: 8px;
  transition: ease 0.5s;
}

/* Track */
::-webkit-scrollbar-track {
  -webkit-border-radius: 10px;
  border-radius: 10px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  -webkit-border-radius: 10px;
  border-radius: 10px;
  background: #404a63;
}

::-webkit-scrollbar-thumb:window-inactive {
  background: #404a63;
  opacity: 0;
}
</style>

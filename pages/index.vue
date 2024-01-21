<template>
  <div>

    <div class="container menu-section">
      <div class="row">
        <div class="col-12">
          <nav class="navbar navbar-light bg-light">
            <div class="container">
              <div class="navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">
                  <li class="nav-item">
                    <nuxt-link to="/auth/login" class="nav-link">Login</nuxt-link>
                  </li>
                  <li class="nav-item">
                    <nuxt-link to="/dashboard" class="nav-link">Dashboard</nuxt-link>
                  </li>
                </ul>
              </div>
            </div>
          </nav>
        </div>
      </div>
    </div>
    <div class="container mt-4">
      <h1>Welcome to LMS</h1>
      <router-view />
    </div>
    <Footer />
  </div>
</template>

<script>

export default {
  components: {

  },
};
</script>

<template>
    <div>
  <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
    <b-navbar-brand href="#" style="font-size:30px;font-weight:bolder ">Skin, Health and Body Shop</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#"></b-nav-item>
        <b-nav-item href="#" disabled></b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search" style="width:350px; border-radius:10px; height:30px"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-4" type="submit" variant="warning">Search</b-button>
        </b-nav-form>

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em style="color: #ffbf00; font-style:normal;">User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
    
</template>


<script>
export default {
    name: "navbar"
}
</script>
<style scoped>

</style>
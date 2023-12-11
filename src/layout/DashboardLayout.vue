<template>
  <div class="wrapper">
    <side-bar class="sidebar">
      <mobile-menu slot="content"></mobile-menu>
      <sidebar-link to="/admin/overview">
        <img src="../../public/img/element-3.png" class="dd">
        <!-- <i class="nc-icon nc-chart-pie-35"></i> -->
        <p>Dashboard</p>
      </sidebar-link>
      <sidebar-link to="/admin/user">
        <img src="../../public/img/bag-2.png" class="dd">
        <!-- <i class="nc-icon nc-circle-09"></i> -->
        <p>Products</p>
      </sidebar-link>
      <sidebar-link to="/admin/table-list">
        <img src="../../public/img/bag-2.png" class="dd">
        <p>Orders</p>
      </sidebar-link>
      <!-- <sidebar-link to="/admin/typography">
        <img src="../../public/img/message-text.png" class="dd">
         <i class="nc-icon nc-paper-2"></i> -->
        <!-- <p>Messages</p> -->
      <!-- </sidebar-link> -->
      <!-- <sidebar-link to="/admin/icons"> -->
        <!-- <i class="nc-icon nc-atom"></i> -->
        <!-- <img src="../../public/img/Vector (1).png" class="dd"> -->
        <!-- <p>Blogs</p> -->
      <!-- </sidebar-link> -->
      <!-- <sidebar-link to="/admin/maps"> -->
        <!-- <i class="nc-icon nc-pin-3"></i> -->
        <!-- <img src="../../public/img/fluent_settings-28-regular.png" class="dd"> -->
        <!-- <p>Settings</p> -->
      <!-- </sidebar-link> --> 

      
      <sidebar-link to="/admin">
        <img src="../../public/img/message-text.png" class="dd">
        <!-- <i class="nc-icon nc-paper-2"></i> -->
        <p>Messages</p>
      </sidebar-link>
      <sidebar-link to="/admin/icons">
        <!-- <i class="nc-icon nc-atom"></i> -->
        <img src="../../public/img/Vector (1).png" class="dd">
        <p>Blogs</p>
      </sidebar-link>
      <sidebar-link to="/admin/maps">
        <!-- <i class="nc-icon nc-pin-3"></i> -->
        <img src="../../public/img/fluent_settings-28-regular.png" class="dd">
        <p>Settings</p>
      </sidebar-link>

     
    </side-bar>
    <div class="main-panel">
      <top-navbar></top-navbar>

      <dashboard-content @click="toggleSidebar">

      </dashboard-content>

      <content-footer></content-footer>
    </div>
  </div>
</template>
<style lang="scss">
   
   .dd{
    width:24px;
    height:24px;
   }

   .wrapper{
    background-color:white !important;
  }
</style>
<script>
  import TopNavbar from './TopNavbar.vue'
  import ContentFooter from './ContentFooter.vue'
  import DashboardContent from './Content.vue'
  import MobileMenu from './MobileMenu.vue'
  export default {
    components: {
      TopNavbar,
      ContentFooter,
      DashboardContent,
      MobileMenu
    },
    methods: {
      toggleSidebar () {
        if (this.$sidebar.showSidebar) {
          this.$sidebar.displaySidebar(false)
        }
      }
    }
  }

</script>

<template>
    <div class="c-app">
      <div class="c-sidebar c-sidebar-dark c-sidebar-fixed" :class="{ 'c-sidebar-lg-show': !$page.url.startsWith('/apps/transactions') }" id="sidebar">
        <div class="c-sidebar-brand d-lg-down-none" style="background: #3c4b64;">
          <img src="/images/medicine.png" class="bg-light rounded shadow-sm p-1" width="35"> <span class="ml-2 font-weight-bold">Sistem Informasi Apotek</span>
        </div>
  
        <!-- sidebar -->
        <Sidebar />
        <!-- end sidebar -->
  
      </div>
      <div class="c-wrapper c-fixed-components">
        
        <!-- header -->
        <Header />
        <!-- end header -->
  
        <div class="c-body">
  
          <!-- content -->
          <slot />
          <!-- end content -->
  
          <footer class="c-footer">
            <div><strong>Sistem Informasi Apotek</strong> &copy; 2024 - Muhamad Rian Rafendi</div>
          </footer>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  
    import Header from '../Components/Header.vue'
    import Sidebar from '../Components/Sidebar.vue'
  
    export default {
  
      //register components
      components: {
        Header,
        Sidebar
      }
  
    }
  </script>
  
  <style>
  </style>
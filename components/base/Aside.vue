<template>
  <aside
    id="layout-menu"
    class="layout-menu-horizontal menu-horizontal menu bg-menu-theme flex-grow-0"
  >
    <div class="container-xxl d-flex h-100">
      <ul class="menu-inner">
    
        <li class="menu-item active">
          <nuxt-link to="/" class="menu-link">
            <Icon name="tdesign:task" class="mx-2"></Icon>
            <div data-i18n="Dashboards">Tareas</div>
          </nuxt-link>
        
        </li>

        <li class="menu-item">
          <nuxt-link to="/users" class="menu-link ">
            <Icon name="tabler:users" class="mx-2"></Icon>
            <div data-i18n="Layouts">Usuarios</div>
          </nuxt-link>

         
        </li>

     
      </ul>
    </div>
  </aside>
</template>

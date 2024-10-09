<template>
  <div class="layout-wrapper layout-navbar-full layout-horizontal layout-without-menu">
    <div class="layout-container">
      <BaseNavbar />
      <div class="layout-page">
        <div class="content-wrapper">
          <BaseAside />
          <div class="container-xxl flex-grow-1 container-p-y">
            <slot/>
          </div>
          <BaseFooter />
          <div class="content-backdrop fade"></div>
        </div>
      </div>
    </div>
  </div>
  <div class="layout-overlay layout-menu-toggle"></div>
  <div class="drag-target"></div>
</template>
<script>
export default {
    name: 'AdminTemplate',
    setup() {
        useHead({
                title: 'Admin',
                bodyAttrs: {
                    dir:"ltr"
                },
                htmlAttrs: {
                  dir:"ltr"   
                },
                link: [
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/fonts/fontawesome.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/fonts/tabler-icons.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/fonts/flag-icons.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/css/rtl/core.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/css/rtl/theme-default.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/css/demo.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/node-waves/node-waves.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/typeahead-js/typeahead.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/fullcalendar/fullcalendar.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/flatpickr/flatpickr.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/select2/select2.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/quill/editor.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/libs/@form-validation/umd/styles/index.min.css',
                        type: 'text/css'
                    },
                    {
                        rel: 'stylesheet',
                        href: '/assets/vendor/css/pages/app-calendar.css',
                        type: 'text/css'
                    }

                ],
                script:[
                    {
                        src:"/assets/vendor/js/helpers.js"
                    },
                          
                    {
                        src:"/assets/js/config.js"
                    },
                    {
                        src:"/assets/vendor/libs/jquery/jquery.js"
                    },
                    {
                        src:"/assets/vendor/libs/popper/popper.js"
                    },
                    {
                        src:"/assets/vendor/js/bootstrap.js"
                    },
                    {
                        src:"/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.js"
                    },
                    {
                        src:"/assets/vendor/libs/node-waves/node-waves.js"
                    },
                    {
                        src:"/assets/vendor/libs/hammer/hammer.js"
                    },
                    {
                        src:"/assets/vendor/libs/i18n/i18n.js"
                    },
                    {
                        src:"/assets/vendor/libs/typeahead-js/typeahead.js"
                    },
                    {
                        src:"/assets/vendor/js/menu.js"
                    },
                    {
                        src:"/assets/vendor/libs/fullcalendar/fullcalendar.js"
                    },
                    {
                        src:"/assets/vendor/libs/@form-validation/umd/bundle/popular.min.js"
                    },
                    {
                        src:"/assets/js/main.js"
                    },
                    {
                        src:"/assets/js/app-calendar-events.js"
                    },
                    {
                        src:"/assets/js/app-calendar.js"
                    }
                
                    
                ]
            }
        )
    }
}
</script>
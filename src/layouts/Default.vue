<template>
  <div class="relative min-h-screen">
    <div class="flex justify-between py-4 mx-2 border-b-2">
      <div>
        <g-link to="/">
          Home
        </g-link>
      </div>

      <div>
        
          <g-link to="/confitures">
          Confitures
        </g-link>
        
      </div>
      <div>
        <a href="https://facebook.com">Facebook</a>
      </div>
      <div>
        <a href="https://instagram.com">Instagram</a>
      </div> 
    </div>
    
    <slot class=""/>

    <g-link to="/A-propos">
      <footer class="absolute bottom-0 w-full h-10 bg-gray-300 hover:bg-gray-400">
        <div class="mt-2 ml-2 text-center">
          <div class="">
            A propos
          </div>
        </div>
      </footer>
    </g-link>
    

  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>


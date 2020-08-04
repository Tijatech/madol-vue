<template>
  <div>
      <header>
                <nav class="desktop">
                    <div class="logo ">
                        <router-link to="/" class="link">MAYOL</router-link>
                    </div>
                    <ul class="nav-links flex w-50">
                        <li><router-link to="/" class="link ">Home</router-link></li>
                        <li><router-link to="/series" class="link">TV Series</router-link></li>
                        <li><router-link to="/movies" class="link">Movies</router-link></li>
                        <li><router-link to="/seasonal" class="link">Seasonal</router-link></li>
                    </ul>
                    <div id="search " class="">
                        <i class="fa fa-search"></i>
                    </div>
                    <div class="user ">
                        <div class="flex ai-c">
                            <img src="https://images.unsplash.com/photo-1488426862026-3ee34a7d66df?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80"
                                class="img-round" alt=""/>
                            <h4 class="p-1">Angelina Joe</h4>    
                        </div>
                    </div>
                </nav>
                <nav class="mobile">
                    <div class="flex justify-sb">
                        <div class="logo ">
                            <router-link to="/" class="link">MAYOL</router-link>
                        </div>
                        <div class="user ">
                            <div class="flex ai-c">
                                <img src="https://images.unsplash.com/photo-1488426862026-3ee34a7d66df?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80"
                                    class="img-round" alt=""/>
                            </div>
                        </div>
                    </div>
                    
                        <ul class="nav-links flex hide-scroll">
                        <li><router-link to="/" class="link ">Home</router-link></li>
                        <li><router-link to="/series" class="link">TV Series</router-link></li>
                        <li><router-link to="/movies" class="link">Movies</router-link></li>
                        <li><router-link to="/seasonal" class="link">Seasonal</router-link></li>
                        </ul>
                   
                
                </nav>
            </header>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>



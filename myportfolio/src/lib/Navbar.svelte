<script>
     const navigation = [
        {name:'A propos de moi', url:'/aboutme'},
        {name:'Formations', url:'/formations'},
        {name:'Expérience', url:'/experience'},
        {name:'Skills&Tools', url:'/skillsandtools'},
        {name:"Contact", url:'/contact'}
    ]
</script>

<div class="navbar-container">
    <nav aria-label="header navigation">
        <a href="/" class="logo" title="Ana Caballero León" aria-label="accueil du site">
        <ul id="menu2" class="links" role="menu" aria-labelledby="menubutton">
            
            {#each navigation as navigations}

            <li role="none">
                <a  role="menuitem" aria-label="Page d'accueil du site" href={navigations.url}>{navigations.name}</a>
            </li>
            {/each}
            
        </ul>

        <button type="button"
            id="menubutton"
            aria-haspopup="true"
            aria-controls="menu2">
            <i class="fa-solid fa-bars"></i>
        </button>
  </nav>

</div>
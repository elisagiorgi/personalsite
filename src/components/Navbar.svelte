<script>
	
	export let menu = 1;
</script>

<style>
    #menu{
         display: flex;
        justify-content: flex-end;
        color: white;
         background: rgba(0, 0, 0, .2);
    }
	ul#menu li{
		display : inline;
        margin: 0 10px;
       
       
	}

    .voice{
        color:white;
    }
    .voice:hover{
        opacity: 0.4
    }
</style>

<ul id="menu">
	<li><a class="voice" href="/" on:click|preventDefault={() => (menu = 1)}>Home</a></li> |
	<li><a class="voice" href="/" on:click|preventDefault={() => (menu = 2)}>About</a></li> |
    	<li><a class="voice" href="/" on:click|preventDefault={() => (menu = 2)}>Skills</a></li>
</ul>

{#if menu === 1}
<!-- <Beranda /> --> Ciaooo
{:else if menu === 2}
<!-- <Profile /> --> ciao
{:else}
<h1>
	Page Not Found
</h1>
{/if}


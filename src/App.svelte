<script>
// import bellLogo from './bell.png';
function handleClick() {
  window.location.href = "https://bell-alliant.vercel.app";
}

</script>

<style>

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;
  height: 100vh;
  width: 100%;
  top: 0;
  left: 0;
}

.logo {
  width: 200px;
  height: 200px;
  margin-bottom: 10px;
}


/* .bell {
  background: #146a9d;
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 800;
  margin: 0;
} */

.black {
  color: black;
  margin: 0;
  text-align: center;
}

.redirect {
  background: black;
  width: 400px;
  color: white;
  border-radius: 2px;
  /* width: 100%; */
  cursor: pointer;
  border: none;
  height: 40px;
  margin-right: 10px;
  margin-left: 10px;
  transform: opacity 0.3s ease-in, box-shadow 0.3s ease-in;
}
  
.redirect:hover {
  opacity: 0.8;
  box-shadow: 1px 1px 1px 1px grey;
}
</style>

<div class="container">
  <div>
    <!-- <h1 class="bell"> Bell </h1>
      -->
    <img class="logo" src="/bell.png" alt="bell"/>
  </div>
  <h1 class="black"> Your e-bill is Ready for review </h1>
  <button class="redirect" on:click={handleClick}> CLICK HERE TO CONTINUE </button>
</div>
<template>
<div>
  <h2>Skills</h2>
<div class="row">

    <div class="left"></div>


    <div class="content">
      
      

    </div>
    

    <div class="right">
        <router-link to="/1" exact><div class="pNo"></div></router-link>
        <router-link to="/2" exact><div class="pNo"></div></router-link>
        <div class="pNo" style="background-color: #92FFBE;"></div>
        <router-link to="/4" exact><div class="pNo"></div></router-link>
        <router-link to="/5" exact><div class="pNo"></div></router-link>
      </div>
</div>


<div class="downArr">
  <img class="animate__animated animate__bounce animate__repeat-2" src="../assets/downArrow.png" alt="">
</div>
  
</div>
</template>

<script>
export default {
  name: ''
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


.row{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  height: 80vh;
  width: 100vw;
  text-align: center
}

.left{
    flex:1;
    max-width: 1;
  }

  .right{
    flex:1;
    max-width: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
  }

  .content{
    flex:8;
    max-width: 8;
    text-align: left;
    padding: 30px;
  }


.pNo{
  width: 20px;
  height: 20px;
  background-color: white;
  border-radius: 50%;
  margin: 15px 30px 15px 0;
}

.downArr{
  position: absolute;
  bottom:10px;
  left: 50%;
  transform: translate(-50%, 0%);
}

.downArr > img{
  width: 10rem;
}

h2{
  text-align: center;
  margin-top: 2rem;
}


@media (max-width: 720px) {

    h2{
        font-size: 1rem;
    }
    .content{
      flex: 100%;
    }

    .left{
      display: none;
    }

    .right{
      display: none;
    }

    .downArr > img{
      width: 7rem;
    }
}

</style>

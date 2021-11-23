<template>
    <div class="home">
      <v-row class="row">
        <v-col class="col" xs="12" sm="12" md="6" lg="6" xl="6">
            <v-card
            class="card rounded-xl pa-2"
            flat
            
  >
            <v-list-item>
            <v-list-item-content>
                
                <v-list-item-title class="text-h5 mb-1 grey--text">
                Hi dears!
                </v-list-item-title>
                <span class="span grey--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad quos consequatur nihil aperiam amet molestiae numquam nobis repellat perferendis doloremque.Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad quos consequatur.</span>
            </v-list-item-content>

            
            </v-list-item>

            <v-card-actions>
            <v-btn
                class="btn pa-3"
                rounded
                text
                router
                to='/portfolio'
            >
                Portfolio
            </v-btn>
            </v-card-actions>
            </v-card>
        </v-col>
        <v-col class="col" xs="12" sm="12" md="6" lg="6" xl="6">
            <div class="img">
             <img id="img" src="../assets/img/dev.png" alt="sorry">
            </div>
        </v-col>
      </v-row>
         

         
    
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
*{
    margin: 0;
}
.home{
    width: 100%;
}

.row{
     margin-top: 140px;
}

.col{
    display: flex;
    justify-content: center;
    
}
.card{
    width: 75%;
    background: rgba(255, 255, 255, 0.698)!important;
    border: none;

}

.span{
    margin: 15px 0;
    font-size: 14px;
    line-height: 1.6!important;
    font-family: 'Arial Narrow Bold', sans-serif;
}
.btn{
    background: rgba(224, 198, 243, 0.315);
    color: rgb(126, 125, 125)!important;
}
.img{
    width: 450px;
    position: relative;
    
}

#img{
  position: absolute;
  top: 0;
  left: 0;
  animation: anim 5s linear infinite;
  width: 100%;
}

@keyframes anim{
  0%{
    top: 0;
  }
  25%{
    top: -30px;
  }
  50%{
    top: 0;
  }
  75%{
    top: 30px;
  }
  100%{
    top: 0;
  }
  
}

</style>
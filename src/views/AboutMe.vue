<template>
    <div class="about">
        
        <div class="wrapBox">

            <div class="square">
                <div class="d"></div>
                <div class="d"></div>
                <div class="d"></div>
            </div>
        </div>
    <v-container>
        <v-row class="mt-0">
            <v-col class="coll" xs="12" sm="12" md="12" lg="12" xl="12">

                <div class="imgCard">

                    <div class="imgBox">
                        <!-- <img src="../assets/img/html2.png" alt="sorry">
                        <img src="../assets/img/html2.png" alt="sorry"> -->
                        <img src="../assets/logo.png" alt="sorry">
                        <img src="../assets/logo.png" alt="sorry">
                    </div>

                    <div class="content">
                        <div class="title"><h5>DIYORA KARIMOVA</h5></div>
                        <div class="subTitle">Hi dears! <br>
                        My name is Diyora, I'm 22 and I'm interested in Web programming. I want to be a strong expert in this speciality.
                        </div>
                        <div class="iconBox">
                            <v-icon class="icon">mdi-facebook</v-icon>
                            <v-icon class="icon">mdi-instagram</v-icon>
                            <v-icon class="icon">mdi-pinterest</v-icon>
                            <v-icon class="icon">mdi-twitter</v-icon>
                        </div>
                    </div>
                </div>
            </v-col>
        </v-row>
    </v-container>

    </div>
</template>

<script>
export default {
    
}
</script>

<style>
.about{
    width: 100%;
    height: 100%;
    position: relative;
    overflow-y: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
}
.wrapBox{
    width: 100%;
    position: absolute;
    top: 0;
    left: -30px;
    
}
.square{
    width: 100%;
    transform: rotate(30deg);
    transform-origin: left;
}
.d{
    width: 100%;
    height: 25px;
    background: rgba(255, 255, 255, 0.548);
    margin: 10px;
}



.imgCard{
    width: 300px;
    height: 400px;
    background-color: rgba(255, 255, 255, 0.007);
    position: relative;
    transform-style: preserve-3d;
    transform: perspective(800px);
    transition: 1s;
    box-shadow: 10px 20px 40px rgba(184, 183, 183, 0.767);
}


.imgCard:hover{
    transform: translateX(50%);
}
.imgCard:hover .imgBox{
            transform: rotateY(-180deg);
        }

.imgBox{
    position: relative;
    width: 100%;
    height: 100%;
    z-index: 1;
    transform-origin: left;
    transform-style: preserve-3d;
    box-shadow: 0px 20px 40px rgba(175, 174, 174, 0.849);
    transition: 1s;
    background: rgba(255, 255, 255, 0.534);
    padding: 15px;
}

img{
    transform-style: preserve-3d;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    width: 100%;
    height: 100%;
    object-fit: fill;
}
img:nth-child(2){
    transform: rotateY(180deg);
}

.content{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 35px;
    background: rgba(255, 255, 255, 0.329);
}

.title{
    font-size: 28px;
    margin-bottom: 20px;
    color: grey;
}

.subTitle{
    font-size: 14px;
    color: grey;
}
.iconBox{
    margin-top: 25px;
    display: flex;
    align-items: center;
}
.iconBox .icon{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 30px;
    height: 30px;
    padding: 8px;
    margin: 5px;
    background-color: rgb(110, 110, 110);
    color: #fff;
    font-size: 16px;
    transition: 0.3s;
    font-size: 20px;
}
.iconBox .icon:hover{
                        background-color: rgba(229, 144, 240, 0.897);
                        cursor: pointer;
}

@media (max-width: 900px)  and (min-width: 600px){
    .imgCard{
        width: 250px;
        height: 300px;
    }

    .content{
        padding: 40px;
    }
}
@media (max-width: 600px)  and (min-width: 400px){
    .imgCard{
        width: 200px;
        height: 250px;
    }

    .content{
        padding: 18px;
    }
    .title{
        font-size: 24px;
        margin-bottom: 15px;
    
    }

    .subTitle{
        font-size: 12px;
    }

    .iconBox .icon{
        width: 25px;
        height: 25px;
        font-size: 14px;
        padding: 5px;
    }
}
@media (max-width: 400px)  and (min-width: 300px){
    .imgCard{
        width: 150px;
        height: 220px;
    }

    .content{
        padding: 14px;
    }
    .title{
        font-size: 14px;
        margin-bottom: 10px;
    
    }

    .subTitle{
        font-size: 10px;
    }

    .iconBox{
        margin-top: 10px;
    }
    .iconBox .icon{
        width: 20px;
        height: 20px;
        font-size: 10px;
    }
}
</style>
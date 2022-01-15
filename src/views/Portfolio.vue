<template>
    <div class="portfolio">
        <v-container class="container">
            <v-row class="row" v-for="ar in arr" :key="ar.id">
                <v-col class="col" xs="12" sm="6" md="6" lg="6" xl="6">
                    <v-card
                    class="card rounded-xl pa-2"
                    flat
                    >
                        <v-list-item>
                        <v-list-item-content>                            
                            <v-list-item-title class="text-h5 mb-1 grey--text text-uppercase">
                            {{ar.name}}
                            </v-list-item-title>
                            <span class="span grey--text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugiat libero dignissimos distinctio magnam ut delectus.</span>
                        </v-list-item-content>
                        </v-list-item>

                        <v-card-actions> 
                        <v-btn
                            class="btn pa-3"
                            rounded
                            text
                        ><a :href="`https://github.com/Diyora19/${ar.url}`" class="grey--text text-decoration-none">
                            source
                        </a>
                            
                        </v-btn>

                        <v-btn 
                            class="btn pa-3"
                            rounded
                            text>
                            <a :href="`https://${ar.show}`" class="grey--text text-decoration-none">
                            show
                            </a>
                        </v-btn>
                        </v-card-actions>
                    </v-card>
                </v-col>
                <v-col xs="12" sm="6" md="6" lg="6" xl="6">
                    <div class="imgBoxx">
                        <img :src="require(`../assets/portfolioImg/${ar.src}`)" alt="sorry">
                       
                        
                    </div>
                </v-col>
            </v-row>
            
        </v-container>
    </div>
</template>

<script>
export default {
    data() {
        return {
            arr:[
                {id:1, name: 'filter-table', src: "filter-table.jpg", url: 'filter_table', show: "filtertablee.netlify.app"},
                {id:2, name: 'filter-cards', src: "filter-cards.jpg", url: 'filter-cards', show: "filterrcard.netlify.app"},
                {id:3, name: 'google-search', src: "google-search.jpg", url: 'google-search', show: "googlesearches.netlify.app"},
                {id:4, name: 'image-animation', src: "img-animation.jpg", url: 'img-animation', show: "imganimation.netlify.app"},
                {id:5, name: 'image-filter', src: "filter-image.jpg", url: 'img-filter', show: "imgfilter.netlify.app"},
                {id:6, name: 'calculation', src: "task-2.jpg", url: 'task-2', show: "simplecalculationpage.netlify.app"},
                {id:7, name: 'img', src: "task-3.jpg", url: 'task-3', show: "selectimg.netlify.app"},
                {id:8, name: 'chat', src: "task-4.jpg", url: 'task-4', show: "makesimplechat.netlify.app"},
                {id:9, name: 'clock', src: "clock.jpg", url: 'clock', show: "coloredclock.netlify.app"},
                {id:10, name: 'football', src: "barsa.jpg", url: 'football', show: "simplefootball.netlify.app"},
                {id:11, name: 'image-contact', src: "imgcontact.jpg", url: 'img-contact', show: "imgcontact.netlify.app"},
                {id:12, name: 'jaisone', src: "jaisone.jpg", url: 'jaisone', show: "jaisone.netlify.app"},
                {id:13, name: 'calculator', src: "calculator.jpg", url: 'calculator', show: "simplegreencalculator.netlify.app"},
                {id:14, name: 'spinner', src: "spinner.jpg", url: 'spinner', show: "simplespinner.netlify.app"},
                {id:15, name: 'website', src: "website.jpg", url: 'website', show: "simpleewebsite.netlify.app"},
                {id:16, name: 'wellsoftpro', src: "wellsoftpro.jpg", url: 'wellsoftpro', show: "wellsoftpro.netlify.app"}
            ],

            
        }
    },
}
</script>

<style lang="scss">
.portfolio{
    .container{
        .row{
            margin: 0;
            .col{
                display: flex;
                justify-content: center;
                align-items: center;
                .imgBoxx{
                    background: rgba(255, 255, 255, 0.698)!important;
                    border-radius: 35px;
                    width: 85%;
                    height: 200px;

                    img{
                        border-radius: 35px;
                        width: 100%;
                        height: 100%;
                        object-fit: cover;
                        position: relative;
                         
                    }
                }
                .card{
                    width: 85%;
                }
            }
        }
    }
}
</style>

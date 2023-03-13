<template>
    
    <section>

        <div class="container">
            <ul class="cards">
                <li v-for="(card, i) in cards"
                 class="card">
                 <figure>

                    <img :src="cards[i].icon" alt="pic">
                 </figure>
                 <h4>{{ cards[i].title }}</h4>
                 <p>{{ cards[i].text }}</p>
                 </li>
            </ul>
        </div>
    </section>

</template>

<script>
export default {
        data(){
            return{
                cards:[
                    {
                        icon:"/src/assets/img/user.png",
                        title: "human capital",
                        text: "Humanizing business: Hamess the power of technology to improve the people work."
                    },
                    {
                        icon:"/src/assets/img/pie-chart.png",
                        title: "core business",
                        text: "It takes innovative approaches to transform, modernize and run existing platforms."
                    },
                    {
                        icon:"/src/assets/img/speedometer.png",
                        title: "performance",
                        text: "Achieving maximum impact and value from investiments in finance and supply chain."
                    },
                ]
            }
        }
}
</script>

<style lang="scss" scoped> 
    section{
        background-color: #eef4ed;
        padding: 8rem 0;

        .cards{
            display: grid;
            grid-template-columns: repeat(3,1fr);
            gap: 26px;
            .card{
                display: flex;
                flex-direction: column;
                row-gap: 23px;
                background-color: white;
                border-radius: 16px;
                padding: 54px 46px;

                figure{
                    padding: 16px;
                    display: flex;
                    text-align: center;
                    width: 64px;
                    aspect-ratio: 1;
                    border-radius: 999px;
                    background-color: #e5f1f1 ;
                    filter: sepia(1) hue-rotate(70deg) saturate(90%) brightness(95%);
                    
                    img{
                        align-self: center;
                        margin: 0 auto;
                    }
                    
                }

                h4{
                    color: #111117;
                }
                
                p{
                    font-size: 18px;
                    color: #111117;
                }
            }
        }
    }
</style>
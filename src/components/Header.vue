<template>
    
    <header>
        <section class="row">
            <div class="header">
                <nav class="row container">
                    <figure class="col-2">
                        <img  src="/src/assets/img/logo.svg" alt="">
                    </figure>
                    <ul class="row">
                        <li v-for="(item, i) in menu"> {{menu[i]}}</li>
                    </ul>
                </nav>  
            </div>
            
            
            <article class="container">
                <h1>Lead ~ <span>Customer</span></h1>
                <p>Succesful strategies require data analysis, creativity and customer focus taking advantage of the latest technologies to offer excellent services.</p>
                <ul class="row">
                    <li>{{ menu[menu.length-1] }}</li>
                    <li>read more</li>
                </ul>
            </article>

            

        </section>

    </header>
    
</template>

<script>
	export default {
        data(){
            return{   
                menu:[
                    "home",
                    "about",
                    "services",
                    "pricing",
                    "blog",
                    "get in touch"
                ]
            }
        }
	}
</script>

<style lang="scss" scoped> 

    header{
        background-image: url("/src/assets/img/hero-image.png");
        background-size: cover;
    }

    section{
        flex-direction: column;
        height: 100vh;
        background-color: rgba(0,0,0,.65);
        
    }

    .header{
        position: sticky;
        top: 0;
        background-color: #21333E ;
        padding: 1.5rem 0;
    }
    
    nav{
        justify-content: space-between;
        align-items: center;

        figure{
            img{
                margin-right: 2rem;
                max-height: 48px;
            }
        }

        ul{
            li{
                text-transform: uppercase;
                margin: 0 1.5rem;
                font-size: 16px;
                line-height: 48px;
                color: white;
            }

            :last-child{
                background-color:#058283;
                padding:0 1.5rem ;
            }
        }
    }

    article{
        flex-grow: 1;
        text-align: center;
        display: flex;
        flex-direction: column;
        justify-content: center;
        
        
        p{
            width: 60%;
            font-size: 18px;
            margin: 0 auto;
        }

        ul{
            margin: 2rem;
            justify-content: center;
            li{
                text-transform: uppercase;
                margin: 0 1.5rem;
                font-size: 16px;
                line-height: 48px;
                color: white;
                border-radius: 4px;
            }

            :first-child{
                background-color:#058283;
                padding:0 1.5rem ;
            }

            :last-child{
                border:#058283 solid 2px;
                padding:0 1.5rem ;
            }
        }
    }

    .center{
        margin-top: auto;
    }
</style>
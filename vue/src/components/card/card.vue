<template>
    <div id="card">
        <img :src="source" />
        <div id="cardText">
            <div id="cardTitle">{{ title }}</div>
            <div id="cardYear">{{ year }}</div>
        </div>
    </div>
</template>

<script>
export default {
    name: "card",
    props:["title", "year", "source"]
}
</script>

<style scoped>
    #card {
        display: flex;
        flex-flow: column nowrap;
        justify-content: space-around;
        align-items: center;
        /* width: 80vw; */
        margin: 20px auto;
        /* height: 500px; */
        min-width: 150px;
        max-width: 200px;
        width: 100%;
        height: auto;
    }
    img {
        width: 85%;
    }
    #cardText {
        font-family: 'Alegreya Sans', sans-serif;
        font-weight: bold;
        width: 100%;
    }
    #cardTitle {
        
        text-align: center;
        padding-top: 20px;
        padding-bottom: 10px;
        height: 40px;
    } 
    #cardYear {
        float: left;
        padding-bottom: 10px;
    } 
    
    /* @media only screen and (min-width: 400px) {
        #card {
            float: left;
            width: 48%;
            margin: 0.5vw;
            height: 411px;
        }
        img {
            width: 85%;
        }
        #cardTitle {
            height: 46px;
        } 
    }
    @media only screen and (min-width: 700px) {
        #card {
            float: left;
            width: 24%;
            margin: 0.5vw;
            height: 380px;
        }
        img {
            width: 100%;
        }
    }
    @media only screen and (min-width: 900px) {
        #card {
            float: left;
            width: 23%;
            margin: 0.5vw;
            height: 400px;
        }
        img {
            width: 100%;
        }
    }
    @media only screen and (min-width: 1200px) {
        #card {
            float: left;
            width: 15%;
            margin: 0.5vw;
            height: 340px;
        }
        img {
            width: 100%;
        }
    }
    @media only screen and (min-width: 2000px) {
        #card {
            height: 520px;
        }
    }
    @media only screen and (min-width: 3000px) {
        #card {
            height: 720px;
            font-size: 2em;
        }
    } */
</style>

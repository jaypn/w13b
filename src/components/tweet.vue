<template>
  <div id="tweet-container">
    <div>
      
      <div id="toggle-button" @click="isGlid=!isGlid">View Tweets</div>
      <p v-if="isGlid">list</p>
      <p v-else>Glid</p>
    </div>
    <div id="tweets" :class="{grid:isGlid,list:!isGlid}">
      <div v-for="tweet in tweets" v-bind:key="tweet.tweet">
        <h2 v-html="tweet.author"></h2>
        <p v-html="tweet.content"></p>
        <p v-html="tweet.date"></p>
      </div>
    </div>
  </div>
</template>

<script 

export default {
    name:"tweetPage",
    
    data: function (){
        return {
            isGlid:true,
            tweets: [
                {
                    author:"Donald Trump"
                    content:"The concept of global warming was created by and for the Chinese in order to make U.S manufacturing non-competititve "
                    date:"Nov 06 2020"
                },
                {
                    author:"Viola Devis"
                    content:"They say to serve is to love. I think to serve is to heal, too"
                    date:"Oct 14 2004"
                },
                {
                    author:"Jayz"
                    content:"I’m not a ‘Business-Man’! I’m a Business… man! Let me handle my business, damn!"
                    date:"Aug 14 2000"
                },
                {
                    author:"kanye West"
                    content:"If it wasn’t for race mixing there’d be no video girls. Me and most of our friends like mutts a lot. Yeah, in the hood they call ’em mutts."
                    date:"Dec 12 2004"
                },
                {
                    author:"Paul Kagame"
                    content:"Let no one think that flexibility and a predisposition to compromise is a sign of weakness or a sell-out."
                    date:"Jun 17 2020"
                },
                {
                    author:"Beyonce"
                    content:"If everything was perfect, you would never learn and you would never grow."
                    date:"Jan 21 2002"
                }
            ] 
        }
    }
}

</script>